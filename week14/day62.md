### mock test 

#### mock
- mock 객체란 모듈의 겉모양이 실제 모듈과 비슷하게 보이도록 만든 가짜 객체 
- 모듈이 필요로하는 의존성이 테스트 케이스 작성을 어렵게 만드는데, 이 의존성을 단절하기 위해 mock 객체가 사용됨 

##### 언제 mock 객체를 만드나? 
- 테스트 작성을 위한 환경 구축이 어려울 때 
- 테스트가 특정 경우나 순간에 의존적일 때 
- 테스트 시간이 오래 걸리는 경우 

##### 테스트 더블 
- 오리지널 객체로 테스트를 진행하기 어려울 경우 이를 대신해 테스트를 진행할 수 있도록 만들어주는 객체 


#### 상태기반 테스트 / 행위 기반 테스트 

##### 상태기반 테스트 
- 특정 메소드를 거친후 객체의 상태에 대해 예상값과 비교하는 방식 

##### 행위기반 테스트 
- 올바른 로직 수행에 대한 판단의 근거로 특정한 동작의 수행 여부를 이용 
- 메소드의 리턴값이 없거나 리턴값을 확인하는 것만으로는 예상대로 동작했음을 보증하기 어려운 경우에 사용 
 
 
 #### mock object 
 - 일반적인 테스트 더블은 상태
 - mock 객체는 행위를 기반으로 테스트 케이스 작성
 
 > mock 객체는 행위를 검증하기 위해 사용되는 객체 지칭
 
 > 행위 기반 테스트는 좀 복잡한 시나리오가 사용되는 경우가 많고, <br>
 모양이나 작성 등 여러 측면에서 어색한 경우가 많아서 만약 상태기반으로 테스트 할 수 있는 상황이라면 굳이 행위 기반 테스트 케이스는 만들지 않는 것이 좋음 
 
 