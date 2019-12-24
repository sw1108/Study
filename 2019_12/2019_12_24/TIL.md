
### Iterator  
- Iterator는 자바의 컬렉션 프레임웍에서 컬렉션에 저장되어있는 요소들을 읽어오는 방법을  
표준화 하였는데 그 중 하나가 Iterator 이다.  
> 자바 컬렉션이란?  
>> 자바에서 대용량의 데이터를 추가/삭제하면서 처리가 필요할 때 사용한다.  
Vector, ArrayList, LinkedList, Set, Map 이 있다.  
>>- Vector : 쓰레드의 개수와 상관없이 동기화 처리를 하지만 싱글 쓰레드 환경에서도 동기화 처리를  
해 성능이 좋지 않아 거의 쓰이지 않는다.  
>>- ArrayList : 배열을 복사하는 방법으로 데이터를 추가/제거한다.  
중간에 데이터를 삽입하면 하나씩 뒤로 밀리기 때문에 데이터의 추가/제거가 많을 경우 오버헤드가 많이
발생한다. 대신 인덱스를 가지고 있어 한번에 원하는 데이터를 접근해 가져올수 있다.
>>- LinkedList : 다음 자료의 정보만 가지고 있고 내부적으로 인덱스는 없는 컬렉션  
추가/삭제가 빈번하게 일어나는 대용양 데이터 처리가 필요할 때 사용(ArrayList와 장단점이 반대)
>>- Set : 순서가 없는 데이터 집합으로 데이터 중복을 허용하지 않는다.
>>- Map : key 와 value 로 구성된 데이터 집합으로 key는 중복이 불가하지만 value는 가능하다.
- Iterator는 인터페이스다.  
```
 // Iterator의 구성
pubilc interface Iterator{
	 boolean hasNext(); 
	Object next();
	void remove();
}
```

> `boolean hasNext()` 메소드는 읽어올 요소가 남아있으면 true, 없으면 false를 반환한다.  
`Object next()` 메소드도 읽어올 요소가 남아있는지 확인하는 메소드로 남아있으면 true,  
없으면 false를 반환한다.  
`void remove()` 메소드는 next()로 읽어온 요소를 삭제한다. 

- Iterator 사용법  
```
Iterator it = list.iterator();
while(it.hasNext()){		// 다음값이 있으면
	list.get(it.next());	// list의 모든 값을 가져온다.
}