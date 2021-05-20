## [Amazon CloudFront](https://docs.aws.amazon.com/ko_kr/AmazonCloudFront/latest/DeveloperGuide/Introduction.html)

Amazon CloudFront는 .html, .css, .js 및 이미지 파일과 같은 **정적 및 동적 웹 콘텐츠를 사용자에게 더 빨리 배포하도록 지원하는 웹 서비스**입니다.

CloudFront를 통해 라우팅 된 Route 53 DNS 요청 및 후속 애플리케이션 트래픽은 인라인으로 검사됩니다.

[Amazon CloudFront 및 Amazon Route 53을 사용하여 DDoS 공격으로부터 동적 웹 애플리케이션을 보호하는 방법](https://aws.amazon.com/ko/blogs/security/how-to-protect-dynamic-web-applications-against-ddos-attacks-by-using-amazon-cloudfront-and-amazon-route-53/)

Amazon CloudFront를 사용해 콘텐츠를 전송하고 웹 애플리케이션의 [**최종 사용자 지연 시간을 단축**](https://aws.amazon.com/ko/getting-started/hands-on/deliver-content-faster/)할 수 있습니다.

## [CloudFront에서 콘텐츠를 제공하는 방법](https://docs.aws.amazon.com/ko_kr/AmazonCloudFront/latest/DeveloperGuide/HowCloudFrontWorks.html)

콘텐츠를 제공하도록 CloudFront를 구성한 후에 사용자가 파일을 요청하면 다음과 같은 결과를 얻습니다.

   * 사용자가 웹 사이트 또는 애플리케이션에 액세스하고 이미지 파일 및 HTML 파일 같은 하나 이상의 파일을 요청합니다.
   * DNS가 요청을 최적으로 서비스할 수 있는 CloudFront POP(엣지 로케이션)로 요청을 라우팅합니다. 이 위치는 일반적으로 지연 시간과 관련해 가장 가까운 CloudFront POP이며, 요청을 엣지 로케이션으로 라우팅합니다.
   * POP에서 CloudFront는 해당 캐시에 요청된 파일이 있는지 확인합니다. 파일이 캐시에 있으면 CloudFront는 파일을 사용자에게 반환합니다. 파일이 캐시에 없으면 다음을 수행합니다.
      * CloudFront는 배포의 사양과 요청을 비교하고 파일에 대한 요청을 해당하는 파일 형식으로 사용자의 오리진 서버(예: 이미지 파일의 경우 Amazon S3 버킷 및 HTML 파일의 경우 HTTP 서버)에 전달합니다.
      * 오리진 서버는 파일을 다시 엣지 로케이션으로 보냅니다.
      * 오리진에서 첫 번째 바이트가 도착하면 CloudFront가 파일을 사용자에게 전달하기 시작합니다. CloudFront는 다음에 다른 사용자가 해당 파일을 요청할 때 엣지 로케이션의 캐시에 파일을 추가합니다.

## 관련 문제

### NO.127 

Which of the following services have Distributed Denial of Service (DDoS) mitigation features? (Select TWO )

-> AWS WAF, Amazon CloudFront

### NO.196 
Users are reporting latency when connecting to an website with a global customer base.<br/>Which AWS service will following can an AWS customer use to launch educing latency?

### NO.222 
A company is building an application that needs to deliver images and videos globally with minimal latency. <br/>Which approach can the company use to accomplish this in a cost effective manner?

-> Deliver the content through Amazon CloudFiont

### NO.228 
Which AWS service securely delivers data, videos , applications, and APIS to users globally with low latency and high transfer speeds?

### NO.246 
A company is planning to launch an ecommerce site in a single AWS Region to a worldwide user base Which AWS services will allow the company to reach users and provide low latency and high transfer speeds? (Select TWO)

-> **AWS Global Accelerator** & **Amazon CloudFront**

### NO.258 
Which AWS service would a customer use with a static website to achieve tower latency and high transfer speeds?
