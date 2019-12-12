## 예외처리 (Exception)
<hr/>

#### 예외 처리 코드  

- 프로그램에서 예외가 발생했을 경우 프로그램의 갑작스러운 종료를 막고,  
정상실행을 유지할 수 있도록 처리하는 코드

``` 
try {
    // 예외가 발생할 수 있는 코드	
} catch (예외종류 참조변수) {

    // 예외 발생 시 처리하는 코드
}
finally {
    // try-catch 블록이 끝나면 무조건 실행되는 블록(생략 가능)
}
```

## 자바 컬렉션  
<hr/>

- Java 컬렉션 프레임워크의 상속구조  

![text](https://t1.daumcdn.net/cfile/tistory/2630264F548D957F09)

- 컬렉션 인터페이스의 특징

| 인터페이스 | 구현클래스 | 특징
|:-----------|:----------:|:------|
| Set | HashSet<br> TreeSet | 순서를 유지하느 않는 데이터의 집합으로 데이터의 중복을 허용하지 않는다 |
|List	|LinkedList<br>Vector<br>ArrayList |순서가 있는 데이터의 집합으로 데이터의 중복을 허용한다|	
|Queue|LinkedList<br>PriorityQueue|List와 유사|
|Map|Hashtable<br>HashMap<br>TreeMap|키(Key),값(Value)의 쌍으로 이루어진 데이터의 집합으로,<br>순서는 유지되지 않으며 키(Key)의 중복을 허용하지 않으나<br>값(Value)의 중복은 허용한다.|


1. Set
> - HashSet
>    - 가장빠른 임의 접근 속도
>    - 순서를 예측할 수 없음
> - TreeSet
>    - 정렬방법을 지정할 수 있음

2. List
> - LinkedList
>	- 양방향 포인터 구조로 데이터의 삽입, 삭제가 빈번할 경우   
> 	 데이터의 위치정보만 수정하면 되기 때문에 사용한다.
> - Vector
>	- 과거에 대용량처리에 사용했으나 내부에서 자동 동기화처리로 비교적 성능이 안좋아 잘쓰이지 않음
> - ArrayList
>	- 단방향 포인터 구조로 각 데이터에 대한 인덱스를 가지고 있어 조회 기능에 성능이 뛰어나다

3. Map
> - Hashtable
>	- HashMap보다는 느리지만 동기화 지원
>	- null 불가
> - HashMap
>	- 중복과 순서가 허용되지 않으며 null값이 올 수 있다.
> - TreeMap
>	- 정렬된 순서대로 키(Key)와 값(Value)을 저장하여 검색이 빠르다.
