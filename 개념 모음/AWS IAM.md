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
   * IAM 그룹
   * IAM 역할
   * IAM의 임시 자격 증명

## IAM 사용자 와 [멀티 팩터 인증(MFA)](https://docs.aws.amazon.com/ko_kr/IAM/latest/UserGuide/id_credentials_mfa.html)

MFA는 사용자가 AWS 웹 사이트 또는 서비스에 액세스할 때 사용자의 **정규 로그인 자격 증명 외에도 AWS가 지원되는 MFA 메커니즘의 고유 인증을 제출하라고 요청**함으로써 **보안을 더욱 강화**합니다.

   * 가상 MFA 디바이스
   * U2F 보안 키
   * 하드웨어 MFA 디바이스
   * SMS 문자 메시지 기반 MFA



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
