## 환경설정

- Java Development Kit (JDK) 설치
- 2가지 환경변수 설정
  - JAVA_HOME
  - PATH
  - 예시
    ```bash
      export JAVA_HOME=/usr/lib/jvm/java-11-openjdk-amd64
      export PATH=$JAVA_HOME/bin:$PATH
    ```

## Java 기본

1. java -version  
   설치된 Java 버전 확인
2. 작성하는 파일의 확장자는 Java
3. 컴파일하게 되면 확장자가 .class로 변경됨
   - 컴파일 명령어: `javac MyFirstClass.java`
4. 컴파일 후 실행
   - 실행 명령어: `java MyFirstClass`
5. Java SE 11부터는 `java` 명령어로 모듈을 실행할 수 있음
   - 컴파일 없이 Java를 실행할 수 있음.
   - 실행 명령어: `java MyFirstClass.java`
