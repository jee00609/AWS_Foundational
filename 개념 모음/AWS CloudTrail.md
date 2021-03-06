## [AWS CloudTrail.md](https://aws.amazon.com/ko/cloudtrail/)

AWS CloudTrail은 AWS 계정의 거버넌스, 규정 준수, 운영 감사, 위험 감사를 지원하는 서비스입니다.

AWS CloudTrail은 사용자 계정에서 이루어진 활동을 기록하고, 로그 파일을 사용자의 Amazon S3 버킷으로 전달하는 웹 서비스입니다.

## CloudTrail 의 이점

CloudTrail은 사용자 계정에서 이루어진 작업을 기록함으로써 사용자 활동에 대한 가시성을 제공합니다.

CloudTrail은 요청한 사람, 사용된 서비스, 수행된 작업, 작업의 파라미터, AWS 서비스에서 반환한 대응 요소를 비롯하여, 각 작업에 대한 중요 정보를 기록합니다.

이러한 정보는 AWS 리소스에 이루어진 변경 사항을 추적하고 운영 관련 문제를 해결하는 데 도움이 됩니다.

## CloudTrail은 누가 사용해야 합니까?

리소스에 대한 변경 사항을 추적하거나, 사용자 활동에 대한 간단한 질문에 답변하거나, 규정 준수를 입증하거나, 문제를 해결하거나, 보안 분석을 수행하려는 고객은 CloudTrail을 사용해야 합니다.

## 참고

[AWS의 Cloudwatch와 CloudTrail의 차이](https://www.enqdeq.net/282)

   * CloudTrail : "AWS에서 **누가** 무엇을합니까?"
      * 서비스 또는 리소스에 대한 API 호출.
      * Who did what on AWS?

   * CloudWatch : "AWS에서 **무슨 일이** 일어나고 있나?" 
      * 특정 서비스 또는 응용 프로그램의 모든 이벤트를 기록합니다.
      * What is happening on AWS?

CloudTrail은 사용장 활동 및 API 사용추적->API 사용추적을 통해 보안 분석 및 문제 해결을

VPC 흐름 로그 -> IP 트래픽에 대한 정보를 수집할 수 있는 기능이다.

Amazon CloudWatch ->애플리케이션 모니터링 사용량 지표,이벤트 운영 데이터 수집을 목표로함.

## 관련 문제

### NO.111 

[EC2 Windows 인스턴스를 중지, 재부팅 또는 종료한 사용자를 찾으려면 어떻게 해야 합니까?](https://aws.amazon.com/ko/premiumsupport/knowledge-center/ec2-windows-identify-stop-reboot/)

Which of the following can be used to identify a specific user who stopped an amazon EC2 instance?
