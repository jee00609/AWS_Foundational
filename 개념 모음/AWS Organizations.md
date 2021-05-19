## [AWS Organizations](https://docs.aws.amazon.com/ko_kr/organizations/latest/userguide/orgs_introduction.html)

AWS Organizations 는 여러 AWS 계정을 사용자가 생성하고 중앙에서 관리하는 단일 조직으로 통합할 수 있는 계정 관리 서비스입니다.

AWS Organizations 기능에는 비즈니스의 예산,보안 및 규정 준수 요구 사항을 더 잘 충족할 수 있는 **계정 관리 및 통합 결제 기능** 이 있습니다.

## AWS Organizations의 통합 결제

AWS Organizations의 통합 결제 기능을 사용하여 여러 AWS 계정 또는 여러 Amazon Internet Services Pvt. Ltd(AISPL) 계정의 결제를 통합할 수 있습니다.

결제를 위해 AWS 는 **조직 내 모든 계정을 하나의 계정처럼 취급**합니다. 

AWS 계정간에 [**예약 인스턴스의 비용 이점을 공유**](https://aws.amazon.com/ko/premiumsupport/knowledge-center/ec2-ri-consolidated-billing/) 할 수 있는 기능을 제공합니다.

AWS 제품 및 서비스는 소규모 신생 기업에서 대기업에 이르기까지 모든 규모의 회사에서 사용할 수 있도록 설계되었습니다. 

회사 규모가 크거나 성장할 가능성이 있는 경우 회사의 구조를 반영하는 여러 AWS 계정을 설정할 수 있습니다. 

예를 들어 회사 전체의 계정 하나와 각 직원의 계정 하나를 만들거나, 회사 전체의 계정 하나를 만들고 각 직원의 IAM 사용자가 있는 계정을 만들 수 있습니다. 회사 전체의 계정, 회사 내 부서별 또는 팀별 계정, 그리고 각 직원의 계정을 만들 수 있습니다.

## [SCP (서비스 제어 정책)](https://docs.aws.amazon.com/organizations/latest/userguide/orgs_manage_policies_scps.html)

SCP(서비스 제어 정책)는 **조직의 권한을 관리**하는 데 사용할 수 있는 조직 정책 유형입니다.

(Service control policies (SCPs) are a type of organization policy that you can use to manage permissions in your organization.)

SCPs 는 조직의 모든 계정에 사용 가능한 최대 권한을 중앙에서 제어합니다.

SCPs 는 [모든 기능이 활성화](https://docs.aws.amazon.com/ko_kr/organizations/latest/userguide/orgs_manage_org_support-all-features.html)된 조직에서만 사용할 수 있습니다.

## 예약 인스턴스

결제를 위해 AWS 조직의 통합 결제 기능은 **조직 내 모든 계정을 하나의 계정으로 취급**합니다. 

즉 조직 내 모든 계정은 다른 계정에서 구입한 예약 인스턴스에 대해 시간당 비용 혜택을 받을 수 있습니다.

RI를 처음 구입한 계정에 우선 할인이 적용됩니다. 

구입 계정에 RI의 조건과 일치하는 인스턴스가 없으면, **조직의 다른 계정에 대한 모든 해당 사용에 RI의 할인이 지정됩니다.**

## 관련 문제

### NO.132 
A company has multiple AWS accounts and wants to simplify and consolidate its billing process.

Which AWS service will achieve this?

### NO.135 
Which AWS service allows for effective cost management of multiple AWS accounts?

### NO.154 
Which of the following provides the ability to share the cost benefits of Reserved Instances across AWS accounts?

### NO.160 
Which methods can be used to identify AWS costs by departments? (Choose two.)

-> **[Create separate accounts for each department](https://docs.aws.amazon.com/ko_kr/awsaccountbilling/latest/aboutv2/awsaccountbilling-aboutv2.pdf)** & **[Use tags to associate each instance with a particular department](https://aws.amazon.com/ko/premiumsupport/knowledge-center/tags-billing-cost-center-project/)**

### NO.166 
A company has multiple AWS accounts within AWS Organizations and wants to apply the Amazon EC2 Reserved instances benefit to a single account only Which action should be taken?

-> [Purchase the Reserved instances in individual linked accounts and turn off Reserved Instance
sharing from the payer level](https://aws.amazon.com/ko/premiumsupport/knowledge-center/ec2-ri-consolidated-billing/)

[](https://www.examtopics.com/discussions/amazon/view/22416-exam-aws-certified-cloud-practitioner-topic-1-question-306/)

### NO.178 
Service control policies (SCPs) manage permissions for which of the following?

-> AWS Organizations

### NO.197 
How can one AWS account use Reserved Instances from another AWS account?

-> By using AWS Organizations consolidated billing

### NO.202 
Which service allows a company with multiple AWS accounts to combine its usage to obtain volume discounts?

### NO.251 
A company's procurement department wants volume discounts on AWS services for the company, but numerous departments have separate AWS accounts.<br/>
Which AWS service or tool can the company use to receive volume discounts across multiple AWS accounts?
