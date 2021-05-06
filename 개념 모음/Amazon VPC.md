## [Amazon VPC](https://docs.aws.amazon.com/ko_kr/vpc/latest/userguide/what-is-amazon-vpc.html)

Amazon Virtual Private Cloud(Amazon VPC)를 이용하면 사용자가 정의한 가상 네트워크로 AWS 리소스를 시작할 수 있습니다. 

## 네트워크 ACL

네트워크 ACL(액세스 제어 목록)은 1개 이상의 서브넷 내부와 외부의 트래픽을 제어하기 위한 방화벽 역할을 하는 VPC를 위한 선택적 보안 계층입니다.

네트워크 ACL 및 보안 그룹 규칙은 **IP 주소가 리소스에 액세스하지 못하도록 허용하거나 차단하는 방화벽 역할**을 합니다.

네트워크 ACL은 서**브넷 수준의 인바운드 및 아웃바운드 트래픽을 제어**합니다.

[**EC2 인스턴스에서 특정 IP를 허용하거나 차단할 때 사용**할 수 있습니다.](https://aws.amazon.com/ko/premiumsupport/knowledge-center/ec2-block-or-allow-ips/)

## 관련 문제

### NO.167 
A company has an AWS environment that consists of a VPC. multiple subnets, and many Amazon EC2 instances in the subnets An engineer wants to restrict inbound traffic to one particular EC2 instance without affecting the other EC2 instances.

A. Network ACLs
