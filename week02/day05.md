#### 오늘 한 일
의뢰 페이지에 몇 컬럼들을 합치는 작업<br>

#### 시행착오
한 칸을 감싸고 있는 <td>안에 또 <td>를 넣으면 될 것이라 간단히 생각했는데 <br>
아예 <tr> 밖에 또 <tr>을 만들어서 두 줄로 만든 후 rowspan을 해야했다.
<br>
```html
또 <thead>와<tbody>를 분리시켜놔서 생각하는게 쉽지 않았다. 
```
<br>

#### 좀 더 공식 문서를 찾아보는 습관을 들이자..
<br>

#### 오늘의 실수 
- 발단
어쩌다 커밋이 두번 되었는데 각 커밋에 올라가면 안되는 파일이 하나씩 끼어서 들어갔고 <br>
그걸 고치려다 revert를 해서 커밋이 3개나 떠있는 아주 정신없는 log가 완성이 되었다. <br>

- 해결
squash 로 여러 커밋을 합칠 수 있다. <br>
git reflog로 삭제된 이력까지 다 볼 수 있다.<br>
브랜치 이동 전에 워킹 디렉토리를 정리하지 않으면 브랜치 이동을 할 수 없다. 
<br>
깃은 자동으로 워킹 디렉토리에 파일들을 추가, 삭제, 수정 해서 checkout 한 브랜치의 마지막 스냅샷으로 되돌려 놓는다. <br>

> git reflog, git stash, ggpush, squash, git rebase

#### 로그를 좀 더 살펴보고 명령어를 치자.. 
