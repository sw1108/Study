#### 자바 스택, 큐  
- 스택(stack) : 마지막에 저장한 가장 먼저 데이터를 꺼낸다.`LIFO` 구조  
- 큐(queue) : 처음에 저장한 데이터를 가장 먼저 꺼내는 `FIFO`구조

- Stack 메서드  

|메서드|설명
|:--|--|
|boolean empty()|스택이 비어있는지 알려준다|
|Object peek()|스택의 맨 위에 저장된 객체를 반환한다.|
|Object pop()|스택의 맨 위에 저장된 객체를 꺼낸다|
|Object push()|스택에 객체를 저장한다.|
|int search(Object p)|스택에 주어진 객체를 찾아서 그 위치를 반환|


- Queue 메서드  

|메서드|설명
|--|--|
|Object element()|삭제없이 저장된 요소를 읽어온다. Queue가 비었을때 exseption발생|
|boolean offer(Object o)|큐에 객체를 저장한다|
|Object peek()|삭제없이 읽어 온다|
|Object poll()|큐에서 꺼내온다. 비었을 때  null반환|
||Object remove()|큐에서 꺼내온다. 비었을 때 Exception 발생|

