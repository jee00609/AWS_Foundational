## [AWS IAM](https://docs.aws.amazon.com/ko_kr/IAM/latest/UserGuide/introduction.html) (AWS Identity and Access Management)

AWS Identity and Access Management(IAM)는 **AWS 리소스에 대한 액세스를 안전하게 제어할 수 있는 웹 서비스**입니다.

 IAM을 사용하여 리소스를 사용하도록 **인증(로그인) 및 권한 부여(권한 있음)된 대상을 제어**합니다.
 
 ## AWS IAM 으로 할 수 있는 것
 
   * [특정 사용자에 대한 Amazon Simple Storage Service (Amazon S3) 버킷 액세스를 제한할 수 있다.](https://aws.amazon.com/ko/premiumsupport/knowledge-center/block-s3-traffic-vpc-ip/)
   * [Amazon S3 버킷의 특정 폴더에 사용자 액세스 권한을 부여하려면 어떻게 해야 합니까?](https://aws.amazon.com/ko/premiumsupport/knowledge-center/s3-folder-user-access/)
 
 ## IAM 자격 증명

   * AWS 계정 루트 사용자
   * IAM 사용자
      * AWS에서 사용자는 이름, AWS Management 콘솔에 로그인할 암호, 그리고 API 또는 CLI와 함께 사용할 수 있는 2개의 액세스 키로 이루어져 있습니다. 
      * **액세스 키 ID**와 **보안 액세스 키**
      * IAM 사용자로 **AWS Management 콘솔에 로그인** 가능합니다.
   * [IAM 그룹](https://docs.aws.amazon.com/ko_kr/IAM/latest/UserGuide/id_groups.html)
      * IAM 사용자 그룹은 IAM 사용자들의 집합입니다.
      * 한 사용자 그룹에 여러 사용자가 포함될 수 있으며 한 사용자가 여러 사용자 그룹에 속할 수 있습니다.
      * 사용자 그룹은 중첩될 수 없습니다. 즉, 사용자 그룹은 사용자만 포함할 수 있으며 다른 사용자 그룹은 포함할 수 없습니다.
      * AWS 계정의 모든 사용자를 자동으로 포함하는 기본 사용자 그룹은 없습니다. 이러한 사용자 그룹이 필요한 경우 하나 만들어 새로운 사용자를 각각 해당 사용자 그룹에 할당해야 합니다.
      * AWS 계정의 IAM 리소스 수와 크기는 제한되어 있습니다. 자세한 내용은 IAM 및 STS 할당량 단원을 참조하세요.
   * IAM 역할
   * IAM의 임시 자격 증명

## IAM 사용자 와 [멀티 팩터 인증(MFA)](https://docs.aws.amazon.com/ko_kr/IAM/latest/UserGuide/id_credentials_mfa.html)

MFA는 사용자가 AWS 웹 사이트 또는 서비스에 액세스할 때 사용자의 **정규 로그인 자격 증명 외에도 AWS가 지원되는 MFA 메커니즘의 고유 인증을 제출하라고 요청**함으로써 **보안을 더욱 강화**합니다.

   * 가상 MFA 디바이스
   * U2F 보안 키
   * 하드웨어 MFA 디바이스
   * SMS 문자 메시지 기반 MFA

## [AWS의 권한 관리 모범 사례](https://kirkpatrickprice.com/blog/best-practices-for-privilege-management-in-aws/)

최소 권한에 대한 모범 사례는 정책에서 가능한 한 최소한의 작업과 리소스 액세스를 허용하도록하는 것입니다.

IAM 정책을 생성 할 때 최소한의 권한으로 시작한 다음 필요한 경우 상승 된 권한을 부여하는 것도 AWS의 권장 사항 입니다. 

또한 IAM 정책은 의도 한대로 작동하는지 확인하기 위해 AWS 환경 및 IAM 정책에 대한 지식이있는 사람이 테스트해야합니다.

## [IAM의 보안 모범 사례](https://docs.aws.amazon.com/ko_kr/IAM/latest/UserGuide/best-practices.html)

   * AWS 계정 루트 사용자 액세스 키 잠금
   * 개별 IAM 사용자 만들기
   * 사용자 그룹을 사용하여 IAM 사용자에게 권한을 할당합니다.
   * 최소 권한 부여
   * AWS 관리형 정책으로 권한 사용 시작
   * 정책 유효성 검사
   * 인라인 정책 대신 고객 관리형 정책 사용
   * 액세스 레벨을 이용한 IAM 권한 검토
   * 사용자에 대한 강력한 암호 정책 구성
   * MFA 활성화
   * Amazon EC2 인스턴스에서 실행되는 애플리케이션에 역할 사용
   * 역할을 사용하여 권한 위임
   * 액세스 키를 공유하면 안 됩니다.
   * 자격 증명을 정기적으로 교체
   * 불필요한 자격 증명 삭제
   * 보안 강화를 위해 정책 조건 사용
   * AWS 계정의 활동 모니터링

## IAM FAQ

### Q: IAM 역할은 무엇입니까?

IAM 역할은 AWS 서비스를 요청하기 위한 권한 세트를 정의하는 IAM 엔터티입니다.

IAM 역할은 특정 사용자나 그룹에 연결되어 있지 않습니다. 

대신 IAM 사용자, 애플리케이션 또는 EC2 같은 AWS 서비스처럼 신뢰할 수 있는 엔터티가 역할을 가정합니다.

## 관련 문제

### NO.161 
Which of the following Identity and Access Management (IAM) entities is associated with an access key ID and secret access key when using AWS Command Line Interface (AWS CLI)?

-> IAM USER

### NO.162 
Which of the following can limit Amazon Simple Storage Service (Amazon S3) bucket access to specific users?

### NO.175 
Which of the following can be used a second factor within the AWS Management Console for AWS Multi-Factor Authentication (AWS MFA)?

-> U2F security key token

### NO.195 
Which of the following identify and access management entitles is associated with an access key id and secret access key when using AWS command line interface?

-> IAM USER

### NO.203 
Which AWS service controls permissions to the AWS management console?

### NO.205 
A company learns that a user's API key has been exposed in a public code repository.<br/> The user has access to sensitive dat a. What is the FIRST step the company should take to ensure the security of its data?

-> [Deactivate the user's API key in AWS Identity and Access Management (IAM)](https://aws.amazon.com/ko/blogs/security/what-to-do-if-you-inadvertently-expose-an-aws-access-key/)

### NO.215 (헷갈림)
The AWS IAM best practice for granting least privilege is to.

-> [apply an IAM policy only to IAM users who require it](https://kirkpatrickprice.com/blog/best-practices-for-privilege-management-in-aws/)

### NO.226 
What are characteristics of AWS IAM users and groups? (Select TWO.)

-> **A user can be a member of multiple groups.** & **Groups can contain users only and cannot be nested.**

### NO.230 
Which of the following are security best practices for using AWS Identity and Access Management (IAM)? (Select TWO)

-> **Rotate credentials regularly** & **Enable multi-factor authentication (MFA)**

### NO.232
According to security best practices, how should an Amazon EC2 instance be given access to an Amazon S3 bucket?

-> Have the EC2 instance assume a role to obtain the privileges to upload the file.

[connect to my Amazon S3 bucket from my Amazon EC2 instance](https://aws.amazon.com/premiumsupport/knowledge-center/ec2-instance-access-s3-bucket/)

### NO.268 
What is an AWS Identity and Access Management (IAM) role?

-> An entity that defines a set of permissions for use with an AWS resource
