### TIL(Today I Learned)  
<hr/>

- 자바 InputStream, OutputStream  
> 자바에서 데이터는 스트림을 통해 입출력 된다.  
단방향 통신을 한다는 특징이 있어 입출력스트림이 따로 필요하다  
데이터 교환에 사용된다


- 자바스크립트 이벤트리스너, 콜백
> 해당 이벤트가 발생했을 때 등록해논 이벤트 리스너가 실행된다  
```
function onClick() {
  alert("클릭클릭");
}

document.getElementById('clickMe').addEventListener('click', onClick); // 이벤트 연결
```

> 이벤트가 실행됐을 때 사용자에게 다시 알려준다.


- onclick 시 
```
<input type="button" class="btn_1"
onclick="upload_btn(${loginMap.member_id})" value="사진 등록" />
```
- 이거처럼 하면 인식을 못하길래 삽질했다
```
<input type="button" class="btn_1"
onclick="upload_btn('${loginMap.member_id}')" value="사진 등록" />
```
-  '' 를 붙여줘서 변수로 만들어줘서 해결