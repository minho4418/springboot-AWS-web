# springboot-web
### AWS를 활용한 Linux기반 웹 서버 구축

# 실행 방법

#### 1. Springboot를 활용하고 html로 웹 생성해주기
#### 2. 위에서 만든 것을 git push 해준다.
#### 3. aws서버에 접속해준다.(xshell을 사용함)
#### 4. Linux기반 서버에서 maven, java, tomcat 설치하고 각각 환경변수를 등록해준다.
#### 5. git clone으로 파일 가져온다.
#### 6. maven실행하면 target폴더에 war파일이 생긴다. 그 war파일을 tomcat/webapps폴더에 붙여넣는다.
#### 7. tomcat/bin에서 start.sh를 입력해 실행시켜준다.
#### 8. 웹주소창에 내가 설정한 주소를 검색해 웹 서비스가 실행되는지 확인한다.

* maven, gradle 아무거나 해도됨
* war가 jar보다 최적화가 더 잘되있기 때문에 사용

오류
setclasspath.sh오류 -> unset CATALINA_HOME
maven 실행 오류 -> https://fors.tistory.com/386
The JAVA_HOME environment variable is not defined correctly 오류 -> source /etc/profile 한번해주면됨.
compiler-plugin:3.8.1:compile 오류 -> <maven.compiler.source>1.8</maven.compiler.source> <maven.compiler.target>1.8</maven.compiler.target> 추가해 주면됨.
