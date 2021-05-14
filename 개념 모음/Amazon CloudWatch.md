## [Amazon CloudWatch](https://aws.amazon.com/ko/cloudwatch/)

Amazon CloudWatch는 DevOps 엔지니어, 개발자, SRE(사이트 안정성 엔지니어) 및 IT 관리자를 위해 구축된 **모니터링 및 관찰 기능 서비스**입니다.

CloudWatch는 애플리케이션을 모니터링하고, 시스템 전반의 성능 변경 사항에 대응하며, 리소스 사용률을 최적화하고, 운영 상태에 대한 통합된 보기를 확보하는 데 필요한 데이터와 실행 가능한 통찰력을 제공합니다.

CloudWatch는 로그, 지표 및 이벤트 형태로 모니터링 및 운영 데이터를 수집하여 AWS와 온프레미스 서버에서 실행되는 AWS 리소스, 애플리케이션 및 서비스에 대한 통합된 보기를 제공합니다.

**Amazon CloudWatch는 Amazon EC2 인스턴스, Amazon DynamoDB 테이블, Amazon RDS DB 인스턴스 같은 AWS 리소스뿐만 아니라 애플리케이션과 서비스에서 생성된 사용자 정의 지표 및 애플리케이션에서 생성된 모든 로그 파일을 모니터링할 수 있습니다.**

## [AWS 계정 루트 사용자 활동 모니터링 및 알림](https://aws.amazon.com/blogs/mt/monitor-and-notify-on-aws-account-root-user-activity/)

AWS 계정 루트 사용자 AWS Management Console 로그인 이벤트에 대한 경고를 모니터링하고 수신하는데 이용 가능하다.

## 참고

[AWS의 Cloudwatch와 CloudTrail의 차이](https://www.enqdeq.net/282)

   * CloudTrail : "AWS에서 **누가** 무엇을합니까?"
      * 서비스 또는 리소스에 대한 API 호출.
      * Who did what on AWS?

   * CloudWatch : "AWS에서 **무슨 일이** 일어나고 있나?" 
      * 특정 서비스 또는 응용 프로그램의 모든 이벤트를 기록합니다.
      * What is happening on AWS?

## 관련 문제

### NO.179 
Which service can be used to monitor and receive alerts for AWS account root user AWS Management Console sign-in events?

### NO.216
[Which AWS service or feature can be used to monitor for potential disk write spikes on a system running on Amazon EC2?](https://aws.amazon.com/ko/blogs/database/how-to-use-cloudwatch-metrics-to-decide-between-general-purpose-or-provisioned-iops-for-your-rds-database/)
