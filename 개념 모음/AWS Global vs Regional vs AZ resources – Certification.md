## [AWS Global vs Regional vs AZ resources – Certification](https://jayendrapatil.com/aws-global-vs-regional-vs-az-resources/)

AWS는 많은 서비스를 제공하며 이러한 서비스는 글로벌, 리전 또는 가용 영역에 한정되며 외부에서 액세스 할 수 없습니다.

대부분의 AWS 관리 형 서비스는 **지역 기반** 서비스입니다.

지역 기반이 아닌 전역 기반 서비스 **(IAM, Route53, CloudFront, WAF 등 제외)**

   * IAM
      * Users, Groups, Roles, Accounts
      * Key Pairs
   * s3
      * Global but Data is Regional
   * Route53
   * WAF
   * CloudFront

## 관련 문제

### NO.121 

Which AWS services are defined as global instead of regional? (Select TWO.)

-> Amazon Route 53 , Amazon CloudFront
