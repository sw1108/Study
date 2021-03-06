## 정리
<hr/>

### 1. 자바의 특징  
- 객체지향언어다
- JVM으로 인해 운영체제에 대해 독립적이다
- 가비지 컬렉션을 통해 자동적으로 메모리를 관리한다.
- 멀티쓰레드를 지원한다.
- 다양한 오픈 라이브러리들이 있다.

### 2. 객체지향 프로그래밍이란? 그 특징   
- 현실의 객체를 필드와 메소드로 정의한 class 기반으로 객체간의 상호작용을 통해  
프로그램이 동작하는것  
##### 특징  
- 코드의 재사용성이 높다
- 상속 : 부모class를 자식이 접근할 수 있도록 물려받는 양식  
- 캡슐화,은닉화 : getter/setter를 사용해 외부 객체에서 구현방식을 알 수 없다.  
- 다형성 : 서로 다른 객체지만 같은 부모의 class 타입으로 관리를 할 수 있다.  

### 3. 오버로딩과 오버라이딩  
- 오버로딩  
	- 같은 이름의 메소드를 여러개 정의하는 것  
	- 매개변수의 타입이나 개수가 달라야 한다.  
- 오버라이딩  
	- 상위 클래스의 메소드를 하위클래스에서 재정의  

### 4. MVC 패턴  
- 데이터와 화면간의 의존 관계를 벗어날 수 있게 하는 개발방법
- Model : 데이터의 처리와 접근을 담당
- View : 사용자에 보여지는 화면을 담당
- Controller: Model 과 View를 제어

### 5. Wrapper Class  
- Primitive type으로 표현할 수 있는 간단한 데이터를 객체로 만들어야 할 경우 사용  

### 6. Servlet, JSP  
- Servlet : 자바로 웹개발을 위해 컨테이너가 이해할 수 있게 순수 자바코드로만 이루어진 것  
- JSP : Servelt에 좀더 접근하기 쉽게하기 위해 html 기반에 자바코드를 블록화 해 삽입한것.

### 7. Session, Cookie  
##### Session  
- 세션에 관련된 데이터는 서버에 저장된다.  
- 웹 브라우저의 캐시에 저장되어 브라우저가 닫히거나 서버에서 삭제시 사라진다.
- 쿠키에 비해 보안성이 좋다.

##### Cookie  
- 사용자가 특정 웹서버에 접속할 때, 생성되는 아이디, 비밀번호, 방문사이트의 정보를 담은  
임시파일로 서버가 아닌 클라이언트에 텍스트 파일로 저장된다.

##### 공통점  
- 웹사이트에서 사용자가 머무르는 동안 상태를 지속 시키기위해 사용자의 정보를 저장한다.  


### 8. Spring Framework  
- 경량 컨테이너로 자바 객체를 직접 관리한다.
	- 라이프 사이클을 관리하며 스프링으로부터 필요한 객체를 얻어올 수 있다.  
- POJO방식의 프레임워크  
	- 일반적인 J2EE 프레임워크에 비해 특정한 인터페이스를 구현하거나 상속받을  
필요가 없어 기존에 존재하는 라이브러리 등을 지원하기 용이하고 객체가 가볍다.  
- IoC(제어 역행)  
	- 컨트롤의 제어권이 사용자가 아니라 프레임워크에 있어서 필요에 따라 스프링에서 사용자의 코드를 호출한다,  
- 의존성 주입(DI)  
	- 객체들 간의 의존성을 줄이기 위해 사용되는 IOC 컨테이너의 구현 방식이다.  
	- 별도의 공간에서 객체를 생성하고 데이터 간의 의존성을 주입하고 개발 코드에서 가져다 쓴다.  
- 관점 지향 프로그래밍(AOP)  
	- 트랜잭션이나 로깅, 보안과 같이 여러 모듈에서 공통적으로 사용하는 기능의 경우 해당 기능을 분리하여 관리하는 방법  
- 영속성과 관련된 다양한 서비스를 지원  
	- 데이터베이스 처리 라이브러리와 연결할 수 있는 인터페이스를 제공한다.  
- 확장성이 높다  

### 9. 쓰레드와 프로세스  
- 쓰레드 : 프로세스내에서 동시에 실행되는 독립적인 실행단위를 말한다.  
- 프로세스 : 운영체제에서 실행중인 하나의 프로그램으로 하나 이상의 쓰레드를 포함한다.  
##### 차이점  
- 프로세스는 서로 메모리 공간을 독자적으로 갖기 때문에 서로 메모리 공간을 공유하지 못한다.  
> 공유하기 위해서는 IPC와 같은 방식을 사용  
- 각 쓰레드는 독자적인 Stack 메모리르 갖고 그 외의 메모리는 프로세스 내에서 공유한다.  

### 10. JVM  
- 자바 가상 머신(JAVA Virtual Machine)의 약자로 JAVA와 OS 사이에서 중개자 역할을 하여  
JAVA가 OS에 구애받지 않고 재사용을 가능하게 해준다.  
- 가장 중요한 메모리관리, 가비지 컬렉션을 수행한다.
