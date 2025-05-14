# jshell

대화형으로 Java 프로그래밍 언어의 선언, 문 및 표현식을 평가하는 도구

```bash
# jshell start
jshell

# 어떤 스니펫을 자동으로 로드했는지 확인하는 명령어
/list -start

# jshell 종료
/exit
```

## jshell 명령어

```console
jshell> int a=4
a ==> 4

jshell> int b=8
b ==> 8

jshell> int square(int i1) {
   ...> return i1 * i1;
   ...> }
|  created method square(int)

jshell> square(b)
$5 ==> 64

jshell> String grade(int testScore) {
...>     if (testScore >= 90) {
...>         return "Pass";
...>     }
...>     return "Fail";
...> }
|  created method grade(int)

jshell> grade(88)
$3 ==> "Fail"

<!-- Overriding -->
jshell> String grade(int testScore) {
...>     if (testScore >= 80) {
...>         return "Pass";
...>     }
...>     return "Fail";
...> }
|  modified method grade(int)

jshell> grade(88)
$5 ==> "Pass"

<!-- Edit IDE -->
jshell> /edit grade
|  modified method grade(int)
jshell> /list grade

   6 : String grade(int testScore) {
           if (testScore >= 85) {
               return "Pass";
           }
           return "Fail";
       }

```
