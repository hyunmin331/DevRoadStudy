# HTTP의 이해

### [**HTTP (Hypertext Transfer Protocol)**](#user-content-fn-1)[^1]

&#x20;HTTP는 HTML 문서와 같은 리소스들을 가져올 수 있도록 해주는 프로토콜로 웹에서 이루어지는 모든 데이터의 교환의 기초

클라이언트-서버 프로토콜 , 수신자 측에 의해 요청이 초기화 되는 프로토콜  &#x20;

주로 클라이언트 서버들은 개별적인 메시지 교환에 의해 통신함

<figure><img src="../.gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>

### HTTP와 HTTPS의 차이(TLS)

HTTPS (_HTTP Secure_) 는 HTTP protocol의 암호화된 버전으로  클라이언트와 서버 간의 모든 커뮤니케이션을 암호화 하기 위하여 SSL 이나 TLS을 사용.&#x20;

이 커넥션은 클라이언트가 민감한 정보를 서버와 안전하게 주고받도록 해줌

TLS를 걸쳐서 HTTP를 사용



ex) 금융 활동, 온라인 쇼핑



### 클라이언트- 서버 모델

* 클라이언트는 주로 요청으로 하고(고객)
* 서버는 이를 처리 후에 응답을 한다(서비스를 제공하는 사람)
* HTTP라는 문서를 통해서 작업이 된다(뭐\~ 주세요 URL사용)

### 무상태

HTTP는 항상 내가 누구인지에대해 알려 주어야 함

각각의 요청에 대해 독립적임

1. 요청과 응답을 통해 계속 주고 받는 쿠키
2. 데이터는 서버에서 관리하고 쿠키 등으로 key를 관리하는 세션
3. 웹 브라우저의 기능 (localStorage 등)

세션 : 서버에서 관리, 키에 대한 값은 쿠키로 주로 관리를 함

쿠키:&#x20;



### HTTP 메세지

![](../.gitbook/assets/image.png)

1. 기본적으로는 사람이 읽을 수 있는 형태
2. 요청과 응답 모두 동일 구조
   1. Start line → 요청과 응답의 형태가 다름.
   2. Headers
   3. 빈 줄
   4. Body
      1. 크기를 알기 어렵다. Headers의 Content-Length 항목 등을 활용한다.
      2. 위와 다르게 꼭 사람이 읽을 수 있는 텍스트 형태일 필요는 없다. 바이너리 등 가능.
      3. 하나가 아니라 여럿일 수도 있다. 파일 업로드 등을 위해 쓰이는 multipart/form-data가 대표적.

[^1]: 
