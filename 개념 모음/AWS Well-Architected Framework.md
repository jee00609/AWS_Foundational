## [AWS Well-Architected Framework](https://aws.amazon.com/ko/architecture/well-architected/)

AWS Well-Architected는 애플리케이션 및 워크로드에 사용할 보안, 성능, 복원력 및 효율성이 뛰어난 인프라를 구축하는 클라우드 아키텍트를 돕기 위해 개발되었습니다.

## AWS Well-Architected 의 5가지 원칙 (Well-Architected 프레임워크의 기반)

   * [운영 우수성 기반](#운영-우수성-기반)
   * [보안 기반](#보안-기반)
   * [안정성 기반](#안정성-기반)
   * [성능 효율성 기반](#성능-효율성-기반)
   * [비용 최적화 기반](#비용-최적화-기반)

## 운영 우수성 기반

운영 우수성 기반에는 비즈니스 가치를 실현하고 지원 프로세스 및 절차를 지속적으로 개선하기 위해 시스템을 실행, 모니터링하고 그에 대한 분석 정보를 얻는 기능이 포함됩니다.

## 보안 기반

보안 기반에는 정보, 시스템, 자산을 보호하는 동시에 위험 진단과 문제 해결 전략을 통해 비즈니스 가치를 제공하는 기능이 포함됩니다.

## 안정성 기반

안정성 기반에는 인프라 또는 서비스 중단으로부터 시스템을 복구하고, 수요를 충족할 컴퓨팅 리소스를 동적으로 확보하며, 잘못된 구성 또는 일시적 네트워크 문제와 같은 중단을 완화하는 기능이 포함됩니다.

## 성능 효율성 기반

성능 효율성 기반에서는 요구 사항 충족을 위한 컴퓨팅 리소스의 효율적인 사용 방식, 그리고 수요가 변화하고 기술이 발전하더라도 우수한 효율성을 유지하는 방법을 중점적으로 설명합니다.

## 비용 최적화 기반

비용 최적화 기반에는 전체 수명 주기 동안 시스템을 개선하고 구체화하는 지속적인 프로세스가 포함됩니다. 최초 개념 증명의 초기 설계부터 지속적인 프로덕션 워크로드 운영에 이르는 전체 과정에 이 백서의 사례를 도입하면 비용을 최소화하면서 원하는 비즈니스 결과를 달성할 수 있는 비용 인식 시스템을 구축하고 운영하여 기업의 투자 수익을 최대화할 수 있습니다.

## AWS Welll-Architected 프레임워크 개념

### 탄력성

필요에 따라 리소스를 획득하고 더 이상 필요하지 않을 때 리소스를 해제하는 기능

탄력성 구현

   * 가변 부하가 있는 워크로드 를 식별합니다 .
   * 작업 부하 범위를 확인합니다 . 즉, 자원 추가 또는 제거를 보증하기에 충분한 가변성이 있습니까?
   * 탄력성을 제한 할 수있는 애플리케이션 제한 (세션, 긴 초기화, 라이선스 등)을 식별합니다.
   * 수요 증가를 자동 확장으로 충족 할 수 있는지 또는 이전에 있어야하는지 확인합니다 ( 이벤트 , 출시 등).
   * Amazon Athena 또는 Amazon Aurora Serverless를 사용할 수있는 애플리케이션 식별
   * 설계 상 탄력적이지 않은 서비스 측면에 대해 AWS Auto Scaling 또는 Application Auto Scaling 을 사용하여 탄력성을 구현 합니다.
   * 탄력성을 위아래로 테스트하여 부하 변동에 대한 요구 사항을 충족하는지 확인합니다.
   * 요구 사항을 충족 할 수있을 때까지 구현 및 테스트를 반복합니다. 골든 Amazon 머신 이미지, 도커 컨테이너 등을 조사하여 시작 속도를 높일 수 있습니다.

### [느슨한 커플링](https://d1.awsstatic.com/whitepapers/AWS_Cloud_Best_Practices.pdf)

IT 구성 요소는 상호 종속성을 줄이도록 설계하여 한 구성 요소의 변경 또는 실패가 다른 구성 요소와 연계되지 않도록 해야 한다는 아키텍처 설계 원칙

애플리케이션 복잡성이 증가함에 따라 IT 시스템의 바람직한 특성은 더 작고 느슨하게 결합 된 구성 요소로 나뉩니다. 

이것은 IT 시스템이 변경 또는 실패와 같은 상호 의존성을 줄이는 방식으로 설계되어야합니다.

**한 구성 요소가 다른 구성 요소에 종속되어서는 안됩니다.**

## 관련 문제

### NO.102

Which pillar of the AWS well-architected framework refers to the ability of a system to recover from infrastructure or service disruptions and dynamically acquire computing resources to meet demand?

### NO.143 

Which AWS Cloud design principles can help increase reliability? (Select TWO.)

[안정성 설계 원칙](https://docs.aws.amazon.com/ko_kr/wellarchitected/latest/reliability-pillar/design-principles.html)

-> Testing recovery procedures, Automatically recovering from failure

   * 장애 자동 복구
   * 복구 절차 테스트
   * 수평적 확장으로 워크로드 전체 가용성 증대
   * 용량 추정 불필요
   * 자동화 변경 사항 관리

### NO.193 
Which scenarios represent the concept of elasticity on AWS? (Choose two.)

-> **Scaling the number of Amazon EC2 instances based on traffic.** & **Resizing Amazon RDS instances as business needs change.**

### NO.194 
IT systems should be designed to reduce interdependencies, so that a change or failure in one component does not cascade to other components This is an example of which principle of cloud architecture design?

-> Loose coupling
