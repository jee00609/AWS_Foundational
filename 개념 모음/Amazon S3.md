## [Amazon S3](https://aws.amazon.com/ko/s3/faqs/)

Amazon S3는 인터넷상 어디서나 원하는 양의 데이터를 저장하고 검색할 수 있도록 구축된 **객체 스토리지**입니다.

Amazon S3는 언제든지 웹상 어디서나 원하는 양의 데이터를 저장하고 검색하는 데 사용할 수 있는 간편한 웹 서비스 인터페이스를 제공합니다.

## Amazon S3 기능

   * 개체를 저장하고
   * 해당 개체에 실시간으로 액세스하며 
   * 버전 관리 및 수명주기 기능을 제공

[Amazon S3 및 Amazon Glacier 의 장점](https://aws.amazon.com/ko/what-is-cloud-object-storage/)

   * 가장 **내구력이 뛰어나고 안정적인 데이터용 플랫폼**
      * 99.999999999% 온라인 내구성을 실현
   * **방대한 규모**에서도 뛰어난 성능
      * 어떠한 용량의 데이터도 저장하고 어디서든 액세스할 수 있도록 지원하므로 애플리케이션을 배포하여 더 많은 사용자에게 더 빨리 접근
   *  **쿼리** 지원
      *  데이터를 추출하고 이를 별도의 분석 시스템으로 로드할 필요 없이 데이터에 바로 정교한 빅 데이터 분석을 실행  
   *  간편하고 유연한 **데이터 전송**
      * S3의 간단하고 안정적인 API를 사용하면 인터넷을 통해 손쉽게 데이터를 전송할 수 있습니다.  
   *  간단하게 사용하는 **강력한 관리 기능**
      * 재정 목표, 준수 규정 및 기업 비즈니스 정책에 맞게 정책을 사용할 수 있습니다.  
   *  가장 포괄적인 **보안 및 규정 준수 기능 세트**
      *  PCI-DSS, HIPAA/HITECH, FedRAMP, SEC Rule 17-a-4, EU 데이터 보호 지침, FISMA 외에도 전 세계 거의 모든 기관에서 다양한 인증을 획득  

## [Amazon S3 종류와 그 비용](https://www.pearsonitcertification.com/articles/article.aspx?p=3004582&seqNum=3)

   * **S3 Standard**: <br/>General-purpose online storage with 99.99% availability and 99.999999999% durability (that is, “11 9s”).

   * **S3 Infrequent Access**: <br/>Same performance as S3 Standard but up to 40% cheaper with 99.9% availability SLA and the same “11 9s” durability.

   * **S3 One Zone-Infrequent Access**: <br/>A cheaper data tier in only one availability zone that can deliver an additional 25% savings over S3 Infrequent Access. It has the same durability, with 99.5% availability.

   * **S3 Reduced Redundancy Storage (RRS)**: <br/>Previously this was a cheaper version of S3 providing 99.99% durability and 99.99% availability of objects. <br/>RRS cannot be used in a life cycling policy and is now more expensive than S3 Standard.

   * **S3 Glacier**: <br/>Less than one-fifth the price of S3 Standard, designed for archiving and long-term storage.

   * **S3 Glacier Deep Archive**: <br/>Costs four times less than Glacier and is the cheapest storage solution, at about $1 per terabyte per month. <br/>This solution is intended for very long-term storage.

## Amazon S3 보안

AWS 고객은 보안에 매우 민감한 조직의 요구 사항에 부합하도록 구축된 데이터 센터 및 네트워크 아키텍처의 혜택을 누릴 수 있습니다.

   * 클라우드의 보안 - AWS는 AWS 클라우드에서 AWS 서비스를 실행하는 인프라를 보호해야 합니다. 
      * 또한 AWS는 안전하게 사용할 수 있는 서비스를 제공해야 합니다. 
      * 서드 파티 감사자는 AWS 규정 준수 프로그램의 일환으로 정기적으로 보안 효과를 테스트하고 검증합니다. 
      * Amazon S3에 적용되는 규정 준수 프로그램에 대한 자세한 내용은 [규정 준수 프로그램 제공 범위 내 AWS 서비스](https://aws.amazon.com/ko/compliance/services-in-scope/)를 참조하십시오.
   * 클라우드 내 보안 - 사용자의 책임은 사용하는 AWS 서비스에 의해 결정됩니다. 
      * 또한 데이터의 민감도, 조직의 요구 사항 및 관련 법률 및 규정을 비롯한 기타 요소에 대해서도 책임이 있습니다.

## 암호화를 사용하여 데이터 보호

Amazon S3에서 데이터 센터의 디스크에 데이터를 쓰면서 객체 수준에서 데이터를 암호화하고 사용자가 해당 데이터에 액세스할 때 자동으로 암호를 해독합니다. 

[암호화 키 관리 방법으로 무엇을 선택하느냐에 따라 다음과 같은 세 가지 옵션을 독립적으로 사용할 수 있습니다.](https://docs.aws.amazon.com/ko_kr/AmazonS3/latest/userguide/serv-side-encryption.html)

   * Amazon S3 관리형 키를 사용한 서버 측 암호화 **(SSE-S3)**
   * AWS Key Management Service에 저장된 고객 마스터 키(CMK)를 사용한 서버 측 암호화 **(SSE-KMS)**
   * 고객 제공 키를 사용한 서버 측 암호화 **(SSE-C)**

## 관련 문제

### NO.113 

Which service stores objects, provides real-time access to those objects, and offers versioning and lifecycle capabilities?

### NO.151 

Which service provides a virtually unlimited amount of online highly durable object storage?

### NO.210 
Which encryption types can be used to protect objects at rest amazon S3?

-> **Server side encryption with S3 managed encryption keys (SSE-S3)** & **Server side encryption with AWS KMS managed encryption keys (SSE KMS)**

### NO.264 
A company is looking for a way to encrypt data stored on Amazon S3. Which AWS managed service can be used to help to accomplish this?

-> AWS Key Management Service (AWS KMS)
