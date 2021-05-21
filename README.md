# 김민혁 [201640208]
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
