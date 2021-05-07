## [AWS CloudFormation](https://docs.aws.amazon.com/ko_kr/AWSCloudFormation/latest/UserGuide/Welcome.html)

AWS CloudFormation은 Amazon Web Services 리소스를 모델링하고 설정하여 **리소스 관리 시간을 줄이고 AWS에서 실행되는 애플리케이션에 더 많은 시간을 사용하도록 해 주는 서비스**입니다. 

필요한 모든 AWS 리소스(예: Amazon EC2 인스턴스 또는 Amazon RDS DB 인스턴스)를 설명하는 템플릿을 생성하면 **AWS CloudFormation이 해당 리소스의 프로비저닝과 구성을 담당**합니다.

**AWS 리소스를 개별적으로 생성하고 구성할 필요가 없으며** 어떤 것이 **무엇에 의존하는지 파악할 필요도 없습니다.**  AWS CloudFormation에서 모든 것을 처리합니다.

AWS CloudFormation 템플릿을 생성하거나 수정할 수 있습니다. 

템플릿에는 모든 리소스와 해당하는 속성이 설명됩니다. 

템플릿을 사용하여 AWS CloudFormation 스택을 생성할 경우 AWS CloudFormation에서 Auto Scaling 그룹, 로드 밸런서 및 데이터베이스를 **자동으로 프로비저닝**합니다.

## AWS CloudFormation을 사용하여 리소스 생성

AWS CloudFormation를 사용하여 GameLift 리소스를 관리할 수 있습니다.

AWS CloudFormation을 사용하면 게임 호스팅을 지원하는 전체 리소스 세트를 관리할 수 있습니다.

AWS CloudFormation에서는 각 리소스를 모델링하는 템플릿을 만든 다음 해당 템플릿을 사용하여 리소스를 생성합니다. 

[CloudFormation StackSets를 사용하여 여러 AWS 계정 및 리전에서 리소스 프로비저닝할 수 있습니다.](https://aws.amazon.com/ko/blogs/aws/use-cloudformation-stacksets-to-provision-resources-across-multiple-aws-accounts-and-regions/)

## 관련 문제

### NO.172 
Which AWS services can be used as infrastructure automation tools? (Select TWO.)

-> **AWS CloudFormation** & **AWS OpsWorks**

### NO.181 
Which AWS service enables users to create copies of resources across AWS Regions?
