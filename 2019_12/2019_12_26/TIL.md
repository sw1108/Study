#### MVC 패턴  

- Model View Controller 의 약자로 어플리케이션을 크게 모델, 뷰, 컨트롤러로 구분하고,  
결합도를 최소화하는 패턴.  

- Model 1  
	- JSP에서 컨트롤러와 뷰 역할을 같이 함.

- Model 2  
	- Servlet은 컨트롤러, JSP는 뷰로 분리되어 사용

- Session
>> 데이터를 담는 request와 session이 있다.
   서버에서 클라이언트에 session을 만들어 보내면 쿠키에 저장한다.
  -  웹페이지에서 로그인을 한 후에 다른 링크를 눌러 페이지가 바뀌어도 
     로그인이 유지되는 이유.
     	- 쿠키를 사용안하는 경우 url뒤에 session을 달고 다닌다.
    	- session은 사용자가 직접 삭제를 안하면 계속 남아있기 때문에 정말 필요한 정보만 사용한다.


#### android  

- 액티비티 생명주기

	- 액티비티가 실행 되면 onCreate(), onStart(), onResume 메소드를 순서대로 호출한다.  
	- 액티비티 실행중 다른 액티비티가 호출되면 onPause(), onStop() 메소드를 순서대로 호출한다.  
	- 이전키를 눌러 액티비티를 종료하면 onPause(), onStop(), onDestroy() 메소드를 순서대로 호출한다.  
	- 다른 액티비티가 호출되었다가 이전으로 돌아오는 경우 onRestart(), onStart(), onResume() 메소드를 차례로 호출한다.  

   
      