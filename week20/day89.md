#### 인스턴스 변수 숨기기 
- 변수를 직접 참조하기 보다는 엑세서 메서드를 통해 접근하는 것이 좋음 

##### 좋지 않은 예 
```ruby 
class Gear 
  def initialize(chainring, cog)
    @chainring =  chainring
    @cog = cog
  end
  
 def ration
  @chainring / @cog.to_f # 변수 직접 참조 : 좋지 않은 예 
 end
end

```

- 주어진 클래스가 직접 선얺나 변수에 접근하더라도 변수를 메서드로 감싸 클래스로부터 감추는게 좋음
- 루비는 캡슐화된 메서드(encapsulating methods) 를 쉽게 만들도록 attr_reader 제공

##### 좋은 예 

```ruby 
class Gear 
  attr_reader :chainring, :cog
  def initialize(chainring, cog)
    @chainring =  chainring
    @cog = cog
  end
  
 def ration
  chainring / cog.to_f # 변수 직접 참조 : 좋지 않은 예 
 end
end

```

- attr_reader 는 변수를 감쌀 수 있는 간단한 래퍼 메서드 만들어 줌
- 아래의 코드가 attr_reader 가 cog 라는 래퍼 메서드를 가상으로 구현한 것 

```ruby
# attr_reader 를 통해 구현
def cog
  @cog
end
```
