# js_study0308
오전 목표 : 포켓몬 기술 완료하고 , 어떤 기능을 지정할 지 정하기 

보안점 
1. num의 개념을 for반복문을 통해 알고있었고 , 다만 식의 마지막에 num ++/ -- 추가해서 포켓몬 캐릭터를 
앞뒤로 이동할수 있는 부분을 알게됐습니다. 
2. 선생님께서 주신 복합대입연산자 키워드를 한번더 생각함!
3. 불러온 이미지와 버튼을 중앙으로 옮겨서 마우스를 클릭시 뒤로 도는모습 연출해보도록 노력중입니다.

절차부분
1. 랜덤으로 버튼을 누르면 앞뒤로 넘어가는 버튼을 두개 생성해주기 (뒷모습값 디폴트)
2. 윗부분은 랜덤이고 포켓몬 생성
3. 아래부분은  6개의 몬스터를 이미지로 채우기   ( 위에 밑에 분담해서 코드합치기)
4. 이미지를 채우고 클릭한 이미지가 윗부분 안으로 랜덤상자에 보이도록 표현하는것 !

( 심화 : 진화과정으로 표현까지 해보고 싶었으나 , 전체포켓몬 개수와 진화구분을 하기어렵다고 판단)

회의과정시 논의 피드백부분
1. 분업시 어떻게 나눠야 할 지 변수같은 설정등 세세한 부분은 어떻게 정할지 의논하였습니다. 
2. 모르는 부분이 있더라도 같이시작하는것을 목표로 하고 ,
3. 이해가지 않는 부분은 동료들과 같은부분을 맡아서 분담하였습니다.
4. 이해해서 다음진도를 나가는 동료들은 다른부분을 나눠서 분담하였습니다.

기술부분 오전시간 
1.  addeventLIstner 클릭이벤트 , 로드이벤트연습필요 하다고 느낀 1줄 동료들 함께 작업했습니다.
2.  div 를 두 구역으로 나눠서 윗 , 아랫부분으로 작게 나눠서 분담한후 중간회의를 가지기로하였습니다.
3.  이제부터 js 파일은 따로만들기로 합의 결정하였습니다. 
기술부분 오후시간 
1.요소: mouseenter 이벤트 
<1> mouseenter 
-mouseTarget.addEventListener("mouseenter", (e) => {
  mouseTarget.style.border = "5px dotted orange";
	  mouseleave
-domElements.img.addEventListener('mouseleave', function(){
  domElements.img.style.border = "5px dotted black";
2.console.log(_PokeData); <- sprites 의 객체 콘솔에서 앞, 뒤의 주소를 받아 설정

3.getElementById().  querySelector() 차이점은? 정확히는 파악하지못했지만
대략 느낌으로는 특정id 를지정하는것과 / 일치하는 그룹들을 지정할때 사용하는 차이인듯 ! 

getElementById()는 무엇인가?
element = document.getElementById(id);
id를 통해 엘리먼트를 반환한다. 
만약 document에 구체적인 ID의 엘리먼트가 없다면 null을 반환한다.

querySelector()는 무엇인가?
element = document.querySelector(selectors);
selector의 구체적인 그룹과 일치하는 document안 첫번째 엘리먼트를 반환한다.
 일치하는게 없으면 null반환한다.
