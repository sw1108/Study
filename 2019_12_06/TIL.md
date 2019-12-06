### 알고리즘 풀기
1. 자연수 N을 입력받아 N의 각 자릿수의 합을 구하자
```
import java.util.*;

public class test {
    public int solution(int n) {
        int answer = 0;
        int sum = 0;
        Scanner scanner = new Scanner(System.in);
        System.out.print("입력:");
        n = scanner.nextInt();
        while(n != 0) {
            sum += n % 10;
            n /= 10;
        }
        
        System.out.println("입력값:" + n + "답:" + sum);

        return answer;
    }
}
```

