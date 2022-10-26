# JavaCode
JAVA 코드 관련

# 수학

## Math

제곱근
```java
Math.sqrt(x)
```
제곱
```java
Math.pow(x, y)
```

# 문자

char 에서의 숫자 판별 = str.charAt(i)-'0'

0123456 -> abcdefg = (char)(str.charAt(i) + 49);

```java
my_string.length() //문자열 길이
my_string.charAt(i)//해당위치 문자 char형이므로 String.valueOf()사용 
my_string.toUpperCase() //대문자 변환
my_string.toLowerCase() //소문자 변환
```

+ Character.isUpperCase()를 사용 대문자인지 구별

+ Character.isLowerCase()를 사용 소문자인지 구별

+ Character.isDigit()를 사용 숫자인지 구별

```java
public static void main(String[] args) {
        char[] chars = {'A', 'a', '1'};
        for (char c : chars) {
            if (Character.isUpperCase(c))
                System.out.println(c + "는 대문자입니다.");
            if (Character.isLowerCase(c))
                System.out.println(c + "는 소문자입니다.");
            if (Character.isDigit(c))
                System.out.println(c + "은 숫자입니다.");
        }
}
//숫자 판별
for(int i = 0 ; i < my_string.length(); i++){
            char value = my_string.charAt(i);
            if(Character.isDigit(value)){
                sum = sum + ((int)value - '0');
            }
        }

```
#### 문자열 비교는 ==가 아닌 equals를 사용해야한다.

### 중복된 문자 제거

```java
 public String solution(String my_string) {
        String answer = "";
        for (int i = 0; i < my_string.length(); i++) {
			if(my_string.indexOf(my_string.charAt(i)) == i){
                answer += my_string.charAt(i);
            }
	}
        return answer;
    }
```

+ indexOf

특정 문자나 문자열이 앞에서부터 처음 발견되는 인덱스를 반환하며 만약 찾지 못했을 경우 "-1"을 반환합니다.


# 배열

```java
arr.length // 
```
