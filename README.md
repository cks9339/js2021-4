# 김민혁 [201640208]
## [05월 25일]
-express 모듈 설치<br>
<pre><code>$ npm install express@4</code></pre>
<h1>요청과응답</h1>
-요청 메시지<br></br>
-응답 메세지

<h1>express 모듈의 기본 메소드</h1>

| 메소드 | 설명 |
|:-----| :------------:|
 |express()| 서버 애플리 케이션 객체를 생성합니다.|
 |app.use()| 요청이 왔을 때 실행할 함수를 지정합니다.|
 |app.listen()| 서버를 실행합니다.|
 <h2>ex)</h2>

 <pre><code>//모듈을 추출합니다.
 const express = require('express');
 
 //서버를 생성합니다.
  const app = express();
  // request 이벤트 리스너를 설정합니다.
  app.use((request, response) =>) {
          response.send('h1 Hello express /h1');
  });
  //서버를 실행합니다
  app.listen(52273, () =>) {
          console.log('Server running at http://127.0.0.1:52273');
  });</code></pre>

  <h1>페이지 라우팅</h1>
  - 클라이언트 요청에 적절한 페이지를 제공하는 기술
  - express 모듈의 페이지 라우팅 메소드

  | 메소드 | 설명 |
  |:-----| :------------:|
 |get(path,callback)| GET요청이 발생했을 때 이벤트 리스너를 지정합니다.|
 |post(path,callback)|  POST요청이 발생했을 때 이벤트 리스너를 지정합니다.|
 |put(path,callback)| PUT요청이 발생했을 때 이벤트 리스너를 지정합니다.|
 |delete(path,callback)| DELETE요청이 발생했을 때 이벤트 리스너를 지정합니다.|
 |all(path,callback)| 모든 요청이 발생했을 때 이벤트 리스너를 지정합니다.|

 <h1>response 객체</h1>

 | 메소드 | 설명 |
|:-----| :------------:|
 |send()| 데이터 본문을 제공합니다.|
 |status()| 상태 코드를 제공합니다.|
 |set()| 헤더를 설정합니다.|

<h1>미들 웨어</h1>

  | 메소드 | 설명 |
|:-----| :------------:|
 |use()| 미들웨어를 설정합니다.|
 - 정적파일 제공<br>
-웹 페이지에서 변경되지 않는 요소들을 쉽게 제공

## [05월 18일]
-Node.js 는 process 전역 객체를 <br></br>
-process 객체는 프로세스 정보를 제공하며, 제어할 수 있게 하는 객체<br></br>
__process 객체의 속성__
| 속성 | 설명 |
| :-----| :------------:|
|env| 컴퓨터 환경 정보를 나타냅니다.|
|version| Node.js 버전을 나타냅니다.|
|versions| Node.js와 종속된 프로그램 버전을 나타냅니다.
|arch| 프로세서의 아키텍처를 나타냅니다.|
|platform| 플랫폼을 나타냅니다.|

__process 객체의 메소드__
| 메소드 | 설명 |
 :-----| :------------:|
|exit([exitCdoe=0])| 프로그램을 종료합니다.|
|memoryUsage()| 메모리 사용 정보를 객체를 리턴합니다.|
|uptime()| 현재 프로그램이 실행된 시간을 리턴합니다.|
-os 모듈 사용
// 모듈을 추출합니다
        const os = require('os');

__os의 메소드__
| 메소드 | 설명 |
 :-----| :------------:|
|hostname()| 운영체제의 호스트 이름을 리턴합니다.|
|type()| 운영체제의 이름을 리턴합니다.|
|playform()| 운영체제의 플랫폼을 리턴합니다.|
|arch()|운영체제의 아키텍처를 리턴합니다.|
|release()|운영체제의 버전을 리턴합니다.|
|uptime()|운영체제가 실행된 시간을 리턴합니다.|
|loadavg()|로드 에버리지 정보를 담은 배열을 리턴합니다.|
|totalmem()|시스템의 총 메모리를 리턴합니다.|
|freemem()|시스템의 사용 가능한 메모리를 리턴합니다.|
|cpus()|CPU의 정보를 담은 객체를 리턴합니다.|
|getNetworkInterfaces()|네트워크 인터페이스의 정보를 담은 배열을 리턴합니다.
|
* url 모듈

        const url - require('url');

* file system 모듈

        const fs = require('fs');
