#visual studio와 github에서 conflict가 발생했을때의 대처법

## 1. 발생원인
visual studio와 github reposistory 문서간 충돌에 의하여 발생된다.
같은 제목의 마크다운 파일에 있어서 수정시각이나 수정상태의 차이에 의하여 충돌된다.

**<예시>** 

(1) 아래 사진은 github에서 작성했을 때 모습

![TEST](/pictures/github1.png)

(2) visual studio에서 작성했을 때 모습

![TEST](/pictures/github2.png)


**= 두 작업의 상태가 다르기 때문에 conflict 발생**

(3) visual studio에서 push가 되지 않는 모습

![TEST](/pictures/github3.png)

(4) <<<head 로 current stage, = 이후로 github에서의 stage를 확인할 수 있다.

![TEST](/pictures/github4.png)

## 2.  해결방법

해당 문제를 해결하기 위해서는 몇 가지 방법을 제시할 수 있다.

**(1) Accept current change**
 작업순서가 더 빠른 current stage를 받아들여 반영할 수 있다.

 **(2) Accept Incoming change**
  이전에 Incoming되었던 stage를 반영하여 작업할 수 있다.

  **(3) Accept both change** 
  두 변화 상태를 모두 반영하여 작업할 수 있다.
  
  **(4) Compare change**
  두 상태의 변화를 비교할 수 있다.

  **(5) 어느 한 쪽의 작업물 삭제**
  충돌이 되는 작업물 중 하나를 임의로 삭제하여 충돌을 해결 할 수 있다. 


 

<br>
<br>

> **참조) 사진을 삽입하는 방법**
>
> 1. 사진 (github.png) 을 harmonylee.github.io/pictures/폴더에 복사한다.
> 2. harmonylee.github.io 폴더위치를 '/' 로 하여 해당하는 사진위치 경로를 구한다. (ex: /pictures/github.png)
 