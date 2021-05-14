## [Shared Responsibility Model (공동 책임 모델)](https://aws.amazon.com/compliance/shared-responsibility-model/?nc1=h_ls)

![공동 책임 모델](https://d1.awsstatic.com/security-center/Shared_Responsibility_Model_V2.59d1eccec334b366627e9295b304202faf7b899b.jpg)


   * **상속된 제어 항목** – 고객이 AWS로부터 전적으로 상속받는 제어 항목.
      * 물리적 및 환경 제어 항목
   * **공유된 제어 항목** – 인프라 계층과 고객 계층에 모두 적용되지만, 컨텍스트 또는 관점이 완벽하게 구분되는 제어 항목. 공유된 제어에서는 AWS는 인프라에 대한 요구 사항을 제공하고 고객은 자사의 AWS 서비스 사용 내에서 자체적인 제어 구현을 제공해야 합니다.
      * 패치 관리 – AWS는 인프라와 관련된 결함 수정과 패치에 대한 책임이 있으며, 고객은 게스트 OS와 애플리케이션 패치에 대한 책임이 있습니다.
      * 구성 관리 – AWS는 인프라 디바이스의 구성을 유지 관리하고, 고객은 자체 게스트 운영 체제, 데이터베이스 및 애플리케이션의 구성에 대한 책임이 있습니다.
      * 인지 및 교육 – AWS는 AWS 직원을 교육하고, 고객은 자사의 직원을 교육해야 합니다.

## 관련 문제

### NO.108 

[How shared responsibility model in AWS security works?](https://www.whizlabs.com/blog/aws-security-shared-responsibility/)

under the AWS shared responsibility model the customer manages which of the following? (AWS 책임 분담 모델에 따라 고객이 다음 중 어떤 것을 관리합니까?)

   * Security group and ACL configuration (보안 그룹 및 ACL 구성)
   * Patch management of an Amazon EC2 instance operating system (Amazon EC2 인스턴스 운영 체제의 패치 관리)

### NO.109 <- 잘모름

Under the AWS shared responsibility model, which task is the customer's responsibility when managing AWS Lambda functions? (AWS 공동 책임 모델에서 AWS Lambda 기능을 관리 할 때 고객의 책임은 무엇입니까?)

[AWS Lambda - The Shared Responsibility Model](https://docs.aws.amazon.com/ko_kr/whitepapers/latest/security-overview-aws-lambda/the-shared-responsibility-model.html)

[Examtopics](https://www.examtopics.com/discussions/amazon/view/43861-exam-aws-certified-cloud-practitioner-topic-1-question-544/)

[AWS Lambda 의 보안 개요](https://buw.medium.com/aws-lambda%EC%9D%98-%EB%B3%B4%EC%95%88-%EA%B0%9C%EC%9A%94-1-2-21a49a9448dc)

**Creating versions of Lambda functions (Lambda 함수 버전 생성)** or **Scaling Lambda resources according to demand (수요에 따라 Lambda 리소스 확장)** 둘 중 하나 인듯하다.

### NO.113 

Which service stores objects, provides real-time access to those objects, and offers versioning and lifecycle capabilities?

(다음 중 AWS에서 전적으로 관리하는 책임 분담 모델의 구성 요소는 무엇입니까?)

   * Auditing physical data center assets (물리적 데이터 센터 자산 감사)
      * Amazon is responsible for auditing physical data center assets and resources since it is the property of Amazon Inc. Customers have no access to physical sites, hence they are not responsible for maintaining physical data center assets.
      *  Amazon은 Amazon Inc.의 자산이므로 물리적 데이터 센터 자산 및 리소스를 감사 할 책임이 있습니다. 고객은 물리적 사이트에 액세스 할 수 없으므로 물리적 데이터 센터 자산을 유지 관리 할 책임이 없습니다.

### NO.123 

According to the AWS shared responsibility model who is responsible for configuration?

[공동 책임 모델](https://aws.amazon.com/ko/compliance/shared-responsibility-model/)

**AWS maintains the configuration of its infrastructure devices, but a customer is responsible for configuring their own guest operating systems, databases, and applications. **

-> It is shared between AWS and the customer

### NO.139 
Which activity is a customer responsibility in the AWS Cloud according to the AWS shared responsibility model?

AWS 책임 분담 모델에 따라 AWS Cloud에서 고객의 책임은 어떤 활동입니까?

-> Ensuring Amazon EBS volumes are backed up (Amazon EBS 볼륨 백업 보장)

### NO.142 
Under the AWS shared responsibility model, customer responsibilities include which one of the following?

AWS 책임 분담 모델에 따라 고객 책임은 무엇인가?

-> Configuring the operating system, network, and firewall. (운영 체제, 네트워크 및 방화벽 구성)

### NO.204 
Which of the following is the responsibility of AWS?

-> Physically destroying storage media at end of life

### NO.206 
A web application is hosted on AWS using an Elastic Load Balancer, multiple Amazon EC2 instances, and Amazon RDS.<br/> Which security measures fall under the responsibility of AWS? (Select TWO.)

-> [**Protecting against IP spoofing and packet sniffing**](https://personal.utdallas.edu/~muratk/courses/cloud11f_files/AWS_Security_Whitepaper.pdf) & [**Installing the latest security patches on the RDS instance**](https://docs.aws.amazon.com/ko_kr/AmazonRDS/latest/UserGuide/UsingWithRDS.html)

-> 참고 <br/>[AWS 는 EC2 인스턴스에 대한 바이러스 백신 보호를 제공하지 않습니다.](https://d1.awsstatic.com/whitepapers/compliance/KO_Whitepapers/AWS_Anitian_Workbook_PCI_Cloud_Compliance_KO.pdf)
<br/>[고객은 데이터 관리(암호화 옵션 포함), 자산 분류, 적절한 허가를 부여하는 IAM 도구 사용에 책임이 있습니다.](https://aws.amazon.com/ko/compliance/shared-responsibility-model/)

### NO.212 
As part of the AWS shared responsibility model, which of the following operational controls do users fully inherit from AWS?

-> Security management of data center

### NO.218 
Under the AWS shared responsibility model, AWS is responsible for which security-related task?

-> Physical security of global infrastructure

### NO.221 
Which of the following tasks is the responsibility of AWS?

-> [Securing the Amazon EC2 hypervisor](https://www.mindpointgroup.com/blog/the-aws-shared-responsibility-model-part-1-security-in-the-cloud/)

(AWS IaaS 오퍼링 인 EC2에서 하이퍼 바이저 계층부터 모든 것이 AWS의 책임입니다.)

### NO.238 
According to the AWS shared responsibility model, which of the following are AWS responsibilities? (Select TWO.)

-> **Network infrastructure and virtualization of infrastructure** & **Physical security of hardware**
