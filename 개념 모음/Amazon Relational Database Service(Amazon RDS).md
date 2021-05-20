## [Amazon Relational Database Service(Amazon RDS)](https://docs.aws.amazon.com/ko_kr/AmazonRDS/latest/UserGuide/Welcome.html)

Amazon Relational Database Service(Amazon RDS)는 AWS 클라우드에서 **관계형 데이터베이스**를 더 쉽게 **설치, 운영 및 확장**할 수 있는 웹 서비스입니다. 

이 서비스는 산업 표준 관계형 데이터베이스를 위한 경제적이고 크기 조절이 가능한 용량을 제공하고 공통 데이터베이스 관리 작업을 관리합니다.

Amazon Relational Database Service(Amazon RDS)를 사용하여 DB 인스턴스를 생성하여 연결이 가능합니다.

**MariaDB, MySQL, Microsoft SQL Server, Oracle 또는 PostgreSQL을 사용하는 DB 인스턴스를 생성**합니다.

## 관련 문제

### NO.213 
What feature of Amazon RDS helps to create globally redundant databases?

(Amazon RDS의 어떤 기능이 전역 중복 데이터베이스를 생성하는 데 도움이 됩니까?)

-> [Cross-Region read replicas](https://aws.amazon.com/ko/blogs/aws/cross-region-read-replicas-for-amazon-rds-for-mysql/) or [Snapshots](https://docs.aws.amazon.com/ko_kr/AWSEC2/latest/UserGuide/EBSSnapshots.html)

[Snapshots 참고 +](https://docs.aws.amazon.com/ko_kr/AmazonRDS/latest/UserGuide/USER_ReadRepl.html)

답은 Cross-Region read replicas 가 더 신빈성있다고 본다.

### NO.257 
Which AWS services can host a Microsoft SQL Server database? (Select TWO.)

-> **Amazon EC2** & [**Amazon Relational Database Service (Amazon RDS)**](https://aws.amazon.com/ko/rds/sqlserver/)
