## [Amazon Route 53](https://docs.aws.amazon.com/ko_kr/Route53/latest/DeveloperGuide/Welcome.html)

Amazon Route 53은 가용성과 확장성이 우수한 **DNS(도메인 이름 시스템) 웹 서비스**입니다.

## Route 53 의 주요 기능

   * **도메인 등록**
      * 웹사이트에는 example.com 같은 이름이 필요합니다. Route 53을 통해 도메인 이름.이라고 하는 웹사이트 또는 웹 애플리케이션의 이름을 등록할 수 있습니다.
   * **DNS 라우팅**
      * 사용자가 웹 브라우저를 열어 주소 표시줄에 도메인 이름(example.com) 또는 하위 도메인 이름(acme.example.com)을 입력한 경우 Route 53은 브라우저를 웹 사이트 또는 웹 애플리케이션에 연결하도록 돕습니다.
   * **상태 확인**
      * Route 53은 인터넷을 통해 웹 서버 같은 리소스로 자동화된 요청을 보내어 접근 및 사용이 가능하고 정상 작동 중인지 확인합니다.
      * 리소스를 사용할 수 없게 될 때 알림을 수신하고 비정상 리소스가 아닌 다른 곳으로 인터넷 트래픽을 라우팅할 수도 있습니다.

3가지 기능을 조합하여 실행 가능하다.

## 관련 문제

### NO.163 
[Which AWS service can help a company detect an outage of its website servers and redirect users to alternate servers?](https://aws.amazon.com/ko/about-aws/whats-new/2013/02/11/announcing-dns-failover-for-route-53/)


