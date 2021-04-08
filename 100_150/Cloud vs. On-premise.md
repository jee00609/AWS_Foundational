## Cloud vs. On-premise

## Cloud

클라우드 컴퓨팅은 IT 리소스를 인터넷을 통해 온디맨드로 제공하고 사용한 만큼만 비용을 지불하는 것을 말합니다.

물리적 데이터 센터와 서버를 구입, 소유 및 유지 관리하는 대신, Amazon Web Services(AWS)와 같은 클라우드 공급자로부터 필요에 따라 컴퓨팅 파워, 스토리지, 데이터베이스와 같은 기술 서비스에 액세스할 수 있습니다.

## On-premise

온프레미스(On-premise)란 기업의 서버를 클라우드 같은 원격 환경에서 운영하는 방식이 아닌, 자체적으로 보유한 전산실 서버에 직접 설치해 운영하는 방식을 의미합니다. 

## 관련 문제

## NO.130
AWS 클라우드와 프레미스 총 소유 비용을 비교할 때 고려해야 할 비용은 무엇입니까?

-> 물리적 스토리지 하드웨어, 데이터 센터의 네트워크 인프라


## NO.131
기존 온 프레미스 솔루션에 비해 AWS Cloud를 사용하면 어떤 이점이 있습니까?

-> 사용자는 향후 용량 요구에 대해 추측 할 필요가 없습니다.

### NO.137 
A company wants to migrate its applications to a VPC on AWS These applications will need to access on-premises resources.

What combination of actions will enable the company to accomplish this goals? (Select TWO )

회사에서 AWS의 VPC로 애플리케이션을 마이그레이션하려고 합니다. 이러한 애플리케이션은 온 프레미스 리소스에 액세스해야 합니다. 회사가 이 목표를 달성할 수 있는 행동 조합은 무엇입니까?

[온 프레미스 네트워크 엔지니어를위한 Amazon VPC – 1 부](https://aws.amazon.com/ko/blogs/apn/amazon-vpc-for-on-premises-network-engineers-part-one/)

   * Build a VPN connection between an on-premises device and a virtual private gateway in the new VPC.
      * (새 VPC에서 온-프레미스 장치와 가상 프라이빗 게이트웨이 간의 VPN 연결을 구축합니다.)
      * [VGW (가상 프라이빗 게이트웨이)를 통해 온 프레미스 데이터 센터에 연결하거나 인터넷 바운드 트래픽에 NAT (Network Address Translation)를 사용합니다.]()

   * Connect the company's on-premises data center to AWS using AWS Direct Connect
      * (AWS Direct Connect를 사용하여 회사의 온 프레미스 데이터 센터를 AWS에 연결합니다.)
      * [VPC 및 VPC 피어링은 단일 지역에 로컬입니다. 지역 간 트래픽은 인터넷, VPN 또는 Direct Connect를 사용하여 연결할 수 있습니다.](https://aws.amazon.com/ko/blogs/apn/amazon-vpc-for-on-premises-network-engineers-part-one/)

### NO.140 
A company is migrating from on-premises data centers to the AWS cloud and is looking for hands-on help with the project.

How can the company get this support? (Select TOO.)

회사는 온 프레미스 데이터 센터에서 AWS 클라우드로 마이그레이션하고 있으며 프로젝트에 대한 실질적인 도움을 찾고 있습니다.

회사는 어떻게 이 지원을 받을 수 있습니까?

[AWS Landing Zone](https://aws.amazon.com/ko/solutions/implementations/aws-landing-zone/)

[AWS Professional Services](https://aws.amazon.com/ko/professional-services/?nc1=h_ls)

   * Use AWS professional services to provide and to set up and AWS Landing Zone in the company's AWS account
      * AWS 전문 서비스를 사용하여 회사의 AWS 계정에서 AWS 랜딩 존을 제공 및 설정

   * Select a partner from the AWS Partner Network (APN) to assist with the migration.
      * AWS 파트너 네트워크 (APN)에서 파트너를 선택하여 마이그레이션을 지원합니다.

