## [Amazon VPC](https://docs.aws.amazon.com/ko_kr/vpc/latest/userguide/what-is-amazon-vpc.html)

Amazon Virtual Private Cloud(Amazon VPC)를 이용하면 사용자가 정의한 가상 네트워크로 AWS 리소스를 시작할 수 있습니다. 

## 네트워크 ACL

네트워크 ACL(액세스 제어 목록)은 1개 이상의 서브넷 내부와 외부의 트래픽을 제어하기 위한 방화벽 역할을 하는 VPC를 위한 선택적 보안 계층입니다.

네트워크 ACL 및 보안 그룹 규칙은 **IP 주소가 리소스에 액세스하지 못하도록 허용하거나 차단하는 방화벽 역할**을 합니다.

네트워크 ACL은 서**브넷 수준의 인바운드 및 아웃바운드 트래픽을 제어**합니다.

[**EC2 인스턴스에서 특정 IP를 허용하거나 차단할 때 사용**할 수 있습니다.](https://aws.amazon.com/ko/premiumsupport/knowledge-center/ec2-block-or-allow-ips/)

## VPC 흐름 로그 (VPC Flow Logs)

VPC 흐름 로그는 **VPC의 네트워크 인터페이스에서 전송되고 수신되는 IP 트래픽에 대한 정보를 수집**할 수 있는 기능입니다. 

플로우 로그 데이터는 Amazon CloudWatch Logs 또는 Amazon S3에 게시될 수 있습니다. 플로우 로그를 생성한 다음 선택된 대상의 데이터를 가져와 확인할 수 있습니다.

   * 지나치게 제한적인 보안 그룹 규칙 진단
   * 인스턴스에 도달하는 트래픽 모니터링
   * 네트워크 인터페이스를 오가는 트래픽 방향 결정

## 관련 문제

### NO.167 
A company has an AWS environment that consists of a VPC. multiple subnets, and many Amazon EC2 instances in the subnets An engineer wants to restrict inbound traffic to one particular EC2 instance without affecting the other EC2 instances.

A. Network ACLs

### NO.249 
Which AWS feature or service can be used to capture information about incoming and outgoing traffic in an AWS VPC infrastructure?

-> VPC Flow Logs
