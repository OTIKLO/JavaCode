# JavaCode
JAVA 코드 관련 vv

## 수학


## 문자

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

##배열

```java
arr.length // 
```
