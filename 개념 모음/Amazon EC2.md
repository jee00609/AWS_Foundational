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

## [Amazon EC2 요금 특징](https://aws.amazon.com/ko/ec2/pricing/?nc1=h_ls)

   * **온디맨드**
      * 선결제 금액이나 장기 약정 없이 저렴하고 유연하게 Amazon EC2를 사용하기 원하는 사용자
      * **단기의 갑작스럽거나 예측할 수 없는 워크로드가 있으며, 중단되어서는 안 되는 애플리케이션**
      * Amazon EC2에서 처음으로 개발 또는 시험 중인 애플리케이션
   * **스팟 인스턴스**
      * **시작 및 종료 시간이 자유로운** 애플리케이션
      * 컴퓨팅 가격이 매우 저렴해야만 수익이 나는 애플리케이션
      * 대량의 서버 용량 추가로 긴급히 컴퓨팅 파워가 필요한 사용자
   * **예약 인스턴스** (+Saving Plans)
      * Savings Plans를 이용해 시간당 USD로 측정되는 **일관된 사용량을 약정**할 수 있습니다.
      * 수요가 꾸준한 애플리케이션
      * 예약 용량이 필요할 수 있는 애플리케이션
      * 총 컴퓨팅 비용을 절감하기 위해 1년 또는 3년 동안 EC2를 사용하기로 약정할 수 있는 고객
   * **전용 호스팅**
      * 전용 호스팅은 고객 전용의 물리적 EC2 서버입니다. 전용 호스팅을 사용하면 Windows Server, SQL Server, SUSE Linux Enterprise Server(라이선스 약관에 따름)를 비롯한 기존 서버 한정 소프트웨어 라이선스를 사용할 수 있으므로 비용을 절감할 뿐 아니라 규정 준수 요구 사항도 충족할 수 있습니다.



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
 
 Amazon EC2 스팟 인스턴스를 사용하면 AWS 클라우드에서 미사용 EC2 용량을 활용할 수 있습니다.
 
 스팟 인스턴스는 온디맨드 요금과 비교하여 **최대 90% 할인된 금액으로 제공**됩니다.
 
 TIP) 예약 인스턴스는 온디맨드 인스턴스 요금과 비교하여 상당한 할인 혜택(최대 75%)을 제공합니다.
 
## AWS 클라우드에서 인프라 호스팅의 이점

   * [사전 약정이 없습니다.](https://aws.amazon.com/ko/about-aws/)
   * 사용자는 필요에 따라 리소스를 프로비저닝할 수 있습니다.

## 데이터베이스

### [Amazon EC2, 이제 Microsoft SQL Server 2019 지원](https://aws.amazon.com/ko/about-aws/whats-new/2019/11/amazon-ec2-now-supports-microsoft-sql-server-2019/)

SQL Server 2019는 오늘부터 모든 AWS 리전에서 사용할 수 있습니다.

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

### NO.171 
Which of the following are benefits of hosting infrastructure in the AWS Cloud? (Choose two.)

-> **There are no upfront commitments.** &  **Users have the ability to provision resources on demand.**

### NO.182
Which Amazon EC2 pricing option is best suited for applications with short-term, spiky, or unpredictable workloads that cannot be interrupted?

-> On-Demand Instances

### NO.185 
A workload on AWS will run for the foreseeable future by using a consistent number of Amazon EC2 instances. What pricing model will minimize cost while ensuring that compute resources remain available?

-> Reserved Instances

### NO.189 
When is it beneficial for a company to use a Spot Instance?

-> When there is flexibility in when an application needs to run.

### NO.252 
A company uses Amazon EC2 infrastructure to host steady-state workloads and needs to achieve significant cost savings.<br/>
Which EC2 instance pricing model should the company select?

-> Reserved Instances

### NO.255 
A company is planning to launch a new steady-state workload on AWS that must be accessible 24 hours a day, 7 days a week. <br/>
What is the MOST cost-effective Amazon EC2 pricing option?

-> On-Demand Instances

### NO.257 
Which AWS services can host a Microsoft SQL Server database? (Select TWO.)

-> **Amazon EC2** & **Amazon Relational Database Service (Amazon RDS)**

### NO.266 
Which Amazon EC2 instance pricing model can provide discounts of up to 90%?

-> Spot Instances

### NO.276 
Which of the following Amazon EC2 pricing models allow customers to use existing serverbound software licenses?

-> Dedicated Hosts
