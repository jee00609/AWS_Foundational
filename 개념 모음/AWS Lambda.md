## [AWS Lambda](https://docs.aws.amazon.com/ko_kr/lambda/latest/dg/welcome.html)

AWS Lambda는 서버를 프로비저닝하거나 관리하지 않고도 코드를 실행할 수 있게 해주는 컴퓨팅 서비스입니다.

 Lambda에서는 사실상 모든 유형의 애플리케이션이나 백엔드 서비스에 대한 코드를 별도의 관리 없이 실행할 수 있습니다.
 
 ## 언제 AWS Lambda 를 사용해야 하는가?
 
 Lambda를 사용하면 사용자는 자신의 코드에 대해서만 책임을 갖습니다.
 
 이 특징을 이용하여 아래와 같은 일을 수행 가능합니다.

   * 용량 프로비저닝, 
   * 플릿 상태 모니터링, 
   * 보안 패치 적용, 
   * 코드 배포, 
   * Lambda 함수 모니터링 및 로깅(과 같은 운영 및 관리 작업)
   
## [AWS 기반 서버리스 서비스](https://aws.amazon.com/ko/serverless/)

   * AWS Lambda
   * Amazon Fargate

## [AWS Lambda 요금](https://aws.amazon.com/ko/lambda/pricing/)

AWS Lambda를 사용하면 사용한 만큼만 비용을 지불합니다. **함수 요청 수**와 **기간**, **코드를 실행하는 데 걸리는 시간**에 따라 요금이 청구됩니다.

Lambda는 콘솔에서 테스트 호출을 포함하여 호출 또는 이벤트 알림에 대한 응답으로 실행을 시작할 때마다 이를 1개 요청으로 계산합니다.

기간은 코드가 실행을 시작한 시간부터 반환되거나 종료될 때까지 시간으로 계산되며, 최대 1밀리초 단위로 반올림됩니다.

(기간은 코드가 실행을 시작한 시간부터 반환되거나 종료될 때까지 시간으로 계산합니다.)

AWS Lambda 프리 티어 사용량에는 월별 무료 요청 1백만 건 및 월별 400,000GB-초 컴퓨팅 시간이 포함됩니다.

## 관련 문제

### NO.152 

Which of the following services is in the category of AWS serverless platform?

### NO.237 
How does AWS charge for AWS Lambda usage once the free tier has been exceeded? (Select TWO)

-> **By the time it takes for the Lambda function to execute.** & **By the number of requests made for a given Lambda function.**
