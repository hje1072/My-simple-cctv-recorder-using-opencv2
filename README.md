# My-simple-cctv-recorder-using-opencv2
opencv의 method들을 이용해 공개된 cctv를 녹화하고, 필터를 넣는 등의 활용을 해보자.


opencv를 이용한 녹화 프로그램
============================
오픈cv에서 제공하는 메소들을 통해 cctv의 정보를 녹화해보고자 한다. <br/> 
내가 사용한 cctv의 정보는 국가에서 제공해주는 공공데이터포털에서 얻은정보이다. <br/> 
정보 출저는 다음과 같다.

  https://www.data.go.kr/data/15063717/fileData.do
  
이 곳에서 다음 cctv 정보를 이용하였다. <br/> 

  #충청남도 천안시 동남구 안서동 506-5 에있는 상명대 입구 삼거리 <br/> 
  'http://210.99.70.120:1935/live/cctv005.stream/playlist.m3u8'<br/> 

코드에서 구현된 기능들 
--------------------------
정확한 정보는 코드내부에 주석을 참고하면 된다. <br/>
이곳에서는 무슨 기능들을 구현했는지 간단히 설명하고자 한다. <br/>

  참고로 프로그램 종료는 esc를 누르면 종료된다. 
* * *
* * *
>프리뷰
>  >  녹화를 진행하기전, cctv의 영상이 나오게 된다. <br/>
>  > 키보드를 통해 아무런 event를 주지않으면 cctv의 영상이 계속 나올 것이다.<br/>


다음 영상은 프리뷰상태에 진입한 프로그램이다. <br/>


https://github.com/hje1072/My-simple-cctv-recorder-using-opencv2/assets/71210590/0ceba45b-dd09-412c-baca-86cd7828070b
* * *
* * *
>녹화
>  >  스페이스바를 누르게 되면 녹화가 진행된다.<br/>
>  > 파이썬파일의 위치에 영상이 녹화된다.<br/>
>  >
>  >   녹화가 되고 있을 경우 화면테두리가 빨간색으로 빛난다. 이를 통해 녹화중임을 확인가능하다.
>  > 
>  > (바탕화면에 파이썬이 있는경우 바탕화면에 저장됨)<br/>
>  > 스페이스바를 두번 누르면 녹화는 종료된다.<br/>
>  >  이미 녹화된 파일이 있을 경우, 새롭게 덮어쓰게 되므로 주의바람.<br/>

다음 영상은 녹화시연이다. <br/>


https://github.com/hje1072/My-simple-cctv-recorder-using-opencv2/assets/71210590/d3da854d-d60f-4c86-a821-be53a69eb85a

* * *
* * *
>필터
>  >  R키를 누르게 되면 화면에서 움직이는 물체의 외형만 나오게 필터를 설정할 수 있다. <br/>
>  > 움직임이 거의 없는 부분은 검정색으로 보일것이며, 움직임이 존재하는 부분은 색깔이 보일것이다.<br/>
>  >  녹화와 같이 R키를 두번 누르면 필터는 꺼진다.<br/>
>  >  필터와 녹화는 동시에 진행될 수 있다.<br/>

다음은 필터시연이다. <br/>



https://github.com/hje1072/My-simple-cctv-recorder-using-opencv2/assets/71210590/364e568f-b5d6-4491-9456-6968c9d2493c


* * *
* * *

>일시정지
>  > P키를 누르면, 화면이 일시정지 된다. 다시한번 P키를 누르면 영상을 다시 재생할 수 있다.<br/>

다음은 일시정지시연이다. <br/>


https://github.com/hje1072/My-simple-cctv-recorder-using-opencv2/assets/71210590/00a26917-b116-4efd-bd1e-bb227f40faf1



