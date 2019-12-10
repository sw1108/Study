### 알고리즘 풀기
<hr/>

1. 길이가 n인 배열을 받아 1부터 n 까지 숫자 중복 x, 한번씩 들어가있는지 확인
```
class Solution {
    public boolean solution(int[] arr) {
        boolean answer = true;
        
        int n = arr.length;		// 배열의 길이
        int a = 0;
        int b = 0;
        for (int i = 0; i < n; i++) {
             a += arr[i];
             b += (i + 1);
        }
        if(a!=b) {
            answer=false;
        }
    
     
        return answer;
    }
}
```


2. 3개의 좌표가 주어지고 직사각형을 만들때 나머지 한점 구하기
```
class Solution {
    public int[] solution(int[][] v) {
       
        int a;
        int b;
        
        if(v[0][0] == v[1][0]) {
            a = v[2][0];
        } else if(v[0][0] == v[2][0]) {
            a = v[1][0];
        } else {
            a = v[0][0];
        }
        
        
        if(v[0][1] == v[1][1]) {
            b = v[2][1];
        } else if(v[0][1] == v[2][1]) {
            b = v[1][1];
        } else {
            b = v[0][1];
        }
        
       int[] answer = {a,b};
        return answer;
    }
}
```

### 툴별 장점
<hr/>

1. STS(SpringSource Tool Suite)
> - 플러그인의 업그레이드 버젼이나 새로운 이클립스 버젼이 나올때마다   
새로운 IDE를 구성해야하는 부담이 없다.
>- 플러그인의 버전 호환성 문제
>- 스프링 팀이 매번 베타버전, RC 버전을 거쳐가면서 플러그인의 호환성  
문제나 버전 이슈를 충분히 검증해준다.
>  - STS는 스프링소스가 제공하는 플러그인 조합이 완료되어있다.

2. 인텔리J(IntelliJ)
> - 다양한 벡엔드&프론트엔드 프로젝트 생성, 자동완성(auto completion),  
>소스코드분석, 지능형리펙토링, 디버거, 테스트러너 기능이 비교된 IDE 중에서  
>가장 우수하기 때문에 개발자의 생산성이 대폭 향상 된다.

3. Eclipse  
> - 플러그인을 필요한 것만 설치하여 편리하게 확장이 가능하다.  
>- 무료다..