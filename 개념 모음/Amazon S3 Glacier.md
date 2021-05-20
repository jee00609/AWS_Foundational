## [Amazon S3 Glacier](https://docs.aws.amazon.com/ko_kr/amazonglacier/latest/dev/introduction.html)

Amazon S3 Glacier는 데이터 보관 및 장기 백업을 위한 안전하고 안정적이며 비용이 매우 저렴한 Amazon S3 스토리지 클래스입니다.

S3 Glacier 고객은 데이터를 수개월, 수년 혹은 수십년까지 비용 효율적으로 저장할 수 있습니다.

S3 Glacier를 통해 스토리지 운영 및 조정에 따른 관리 부담을 AWS에게 이관하여 아래와 같은 일들을 걱정할 필요가 없습니다.

   * 용량 계획
   * 하드웨어 프로비저닝
   * 데이터 복제
   * 하드웨어 장애 탐지 및 복구
   * 시간이 오래 걸리는 하드웨어 마이그레이션 

비용을 낮게 유지하면서 동시에 다양한 검색 요구를 지원하기 위해 Amazon S3 Glacier에서는 아카이브에 액세스하는 3가지 옵션(몇 분에서 몇 시간까지 소요)을 제공하며 S3 Glacier Deep Archive는 2가지 액세스 옵션(12~48시간 소요)을 제공합니다.

## 비용 비교

   * S3 Standard - Infrequent Access * - For long lived but infrequently accessed data that needs millisecond access
      * All Storage / Month $0.0125 per GB
   * S3 One Zone - Infrequent Access * - For re-createable infrequently accessed data that needs millisecond access
      * All Storage / Month $0.01 per GB
   * S3 Glacier ** - For long-term backups and archives with retrieval option from 1 minute to 12 hours
      * All Storage / Month $0.004 per GB

## 관련 문제

### NO.117 

A Cloud Practitioner needs to store data for 7 years to meet regulatory requirements. Which AWS service will meet this requirement at the LOWEST cost?

### NO.157 
A company is building a new archiving system on AWS that will store terabytes of data. 
<br/>The company will NOT retrieve the data often. Which Amazon S3 storage class will MINIMIZE the cost of the system?

### NO.291 
A bank needs to store recordings of calls made to its contact center tor 6 years. <br/>
The recordings must be accessible within 48 hours from the time they are requested.<br/>
Which AWS service will provide a secure and cost-effective solution for retaining these files?
