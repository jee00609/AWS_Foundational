## [AWS Trusted Advisor](https://aws.amazon.com/ko/premiumsupport/technology/trusted-advisor/)

AWS Trusted Advisor는 AWS 모범 사례에 따라 리소스를 프로비저닝하는 데 도움이 되도록 실시간 지침을 제공하는 온라인 도구입니다.

Trusted Advisor는 **AWS 인프라를 최적화**하고 **보안과 성능을 향상**시키고 **전체 비용을 절감**하며 **서비스 한도를 모니터링**할 수 있습니다.

AWS Trusted Advisor는 지금까지 수많은 AWS 고객에게 제공된 AWS의 축적된 서비스 경험에서 얻은 유용한 모범 사례를 바탕으로 만들어진 애플리케이션입니다. 

Trusted Advisor는 사용자의 AWS 환경을 조사하고 비용 절감, 시스템 성능 향상 또는 보안 결함 제거를 위한 권장 사항을 제시합니다.

## [AWS Trusted Advisor 모범 사례 체크리스트](https://aws.amazon.com/ko/premiumsupport/technology/trusted-advisor/best-practice-checklist/)

   * [비용 최적화](#비용-최적화)
   * [보안](#보안)
   * [내결함성](#내결함성) 
   * [성능](#성능)
   * [서비스 한도](#서비스-한도)


## 비용 최적화

**Amazon EC2 인스턴스, Amazon Elastic Block Store (Amazon EBS) 볼륨 및 Amazon RDS 데이터베이스와 같은 AWS 리소스의 크기를 조정하기위한 권장 사항을 제공**

## 보안

결함을 없애고, 다양한 AWS 보안 기능을 사용하며, 권한을 점검하여 애플리케이션 보안을 개선합니다.

   * **특정 포트에 대한 제한 없는 액세스**(0.0.0.0/0)를 허용하는 규칙에 대해 보안 그룹을 점검
   * 리소스에 제한 없는 액세스를 허용하는 규칙에 대해 보안 그룹을 점검
   * (IAM)의 사용을 점검
   * 일반에 노출된 액세스 키가 있는지 그리고 손상된 액세스 키로 인해 비정상적으로 사용된 Amazon Elastic Compute Cloud(Amazon EC2)가 있는지 널리 사용되는 코드 리포지토리를 점검

등등이 있습니다.

AWS Basic Support 및 AWS Developer Support 고객은 6회의 보안 점검(S3 버킷 권한, 보안 그룹 - 특정 포트 무제한, IAM 사용, 루트 계정의 MFA, EBS 퍼블릭 스냅샷, RDS 퍼블릭 스냅샷)과 50회의 서비스 한도 점검에 액세스할 수 있습니다.

## 내결함성

Auto Scaling, 상태 확인, 다중 AZ 및 백업 기능을 활용하여 AWS 애플리케이션의 가용성과 중복성을 높입니다.

## 성능

서비스 한도를 점검하고, 프로비저닝된 처리량을 활용하는지 확인하고, 과다 사용되는 인스턴스를 모니터링하여 서비스 성능을 개선합니다.

## 서비스 한도

서비스 한도의 80%가 넘는 서비스 사용량이 있는지 점검합니다. 

값은 스냅샷을 기반으로 하므로 현재 사용량은 다를 수 있습니다. 한도 및 사용량에 변경 사항이 반영되는 데 최대 24시간이 걸릴 수 있습니다.

## 관련 문제

### NO.129

Which AWS service provides recommendations for rightsizing AWS resources such as Amazon EC2 instances, Amazon Elastic Block Store (Amazon EBS) volumes and Amazon RDS databases to help users reduce costs?

### NO.153 

To avoid malicious compute activities, a user needs a quick way to determine if any Amazon EC2 instances have ports that allow Unrestricted access.<br/>Which AWS service will support this requirement?



