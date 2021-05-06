## [Amazon EC2 (Amazon Elastic Compute Cloud)](https://docs.aws.amazon.com/ko_kr/AWSEC2/latest/UserGuide/concepts.html)

Amazon Elastic Compute Cloud(Amazon EC2)는 크기를 조정할 수 있는 컴퓨팅 용량을 제공하는 웹 서비스입니다.

(컴퓨팅 용량이란 말 그대로, 소프트웨어 시스템 구축 및 호스팅에 사용하는 Amazon 데이터 센터의 서버를 의미합니다.)

## Amazon EC2가 제공하는 기능

   * 인스턴스: 가상 컴퓨팅 환경

   * Amazon 머신 이미지(AMI): 서버에 필요한 운영체제와 여러 소프트웨어들이 적절히 구성된 상태로 제공되는 템플릿으로 인스턴스를 쉽게 만들 수 있습니다.

   * 인스턴스 유형: 인스턴스를 위한 CPU, 메모리, 스토리지, 네트워킹 용량의 여러 가지 구성 제공

   * 키 페어를 사용하여 인스턴스 로그인 정보 보호(AWS는 퍼블릭 키를 저장하고 사용자는 개인 키를 안전한 장소에 보관하는 방식)

   * 인스턴스 스토어 볼륨: 임시 데이터를 저장하는 스토리지 볼륨으로 인스턴스 중단, 최대 절전 모드로 전환 또는 종료 시 삭제됨

   * Amazon Elastic Block Store(Amazon EBS), 즉 Amazon EBS 볼륨을 사용해 영구 스토리지 볼륨에 데이터 저장

   * 인스턴스와 Amazon EBS 볼륨 등의 리소스를 다른 물리적 장소에서 액세스할 수 있는 리전 및 가용 영역

   * 보안 그룹을 사용해 인스턴스에 연결할 수 있는 프로토콜, 포트, 소스 IP 범위를 지정하는 방화벽 기능

   * 탄력적 IP 주소(EIP): 동적 클라우드 컴퓨팅을 위한 고정 IPv4 주소

   * 태그: 사용자가 생성하여 Amazon EC2 리소스에 할당할 수 있는 메타데이터

   * AWS 클라우드에서는 논리적으로 격리되어 있지만 원할 때마다 고객의 네트워크와 간편히 연결할 수 있는 가상 네트워크인 Virtual Private Clouds(VPC)

## 인스턴스 구입 옵션

   * **온디맨드 인스턴스** - 시작하는 인스턴스에 대한 비용을 초 단위로 지불합니다.

   * **Savings Plans** – 1년 또는 3년 기간 동안 시간당 USD로 일관된 사용량을 약정하여 Amazon EC2 비용을 절감할 수 있습니다.

   * **예약 인스턴스** – 1년 또는 3년 기간 동안 인스턴스 유형 또는 지역을 포함해 일관된 인스턴스 구성을 약정하여 Amazon EC2 비용을 절감할 수 있습니다.

   * **스팟 인스턴스** – 미사용 EC2 인스턴스를 요청하여 Amazon EC2 비용을 대폭 줄일 수 있습니다.

   * **전용 호스트** - 인스턴스 실행을 전담하는 실제 호스트 비용을 지불하며, 기존의 소켓, 코어 또는 VM 소프트웨어별 라이선스를 가져와 비용을 절감합니다.

   * **전용 인스턴스** - 단일 테넌트 하드웨어에서 실행되는 인스턴스 비용을 시간 단위로 지불합니다.

   * **용량 예약** – 원하는 기간 동안 특정 가용 영역의 EC2 인스턴스에 대해 용량을 예약합니다.

## [스팟 인스턴스와 온디맨드 인스턴스의 차이점](https://docs.aws.amazon.com/ko_kr/AWSEC2/latest/UserGuide/using-spot-instances.html)

 스팟 인스턴스는 용량을 더 이상 사용할 수 없거나 스팟 가격이 최고 가격을 초과하거나 스팟 인스턴스에 대한 수요가 증가하는 경우 Amazon EC2 스팟 서비스에서 개별 스팟 인스턴스을 중단할 수 있습니다.

## 관련 문제

### NO.116 

Which AWS service allows customers to purchase unused Amazon EC2 capacity at an often discounted rate?

-> Spot Instances

### NO.118 

Which of the following AWS Cloud services can be used to run a customer-managed relational database?

(고객 관리 형 관계형 데이터베이스를 실행하는데 사용할수 있는 AWS 클라우드 서비스)

-> Amazon EC2

### NO.169 
Which pricing model will interrupt a running amazon EC2 instance if capacity becomes temporarily unavailable?

-> Spot Instances
