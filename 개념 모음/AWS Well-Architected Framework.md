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
