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

## [퍼블릭 및 프라이빗 서브넷이 있는 VPC(NAT)](https://docs.aws.amazon.com/ko_kr/vpc/latest/userguide/VPC_Scenario2.html)

퍼블릭 서브넷의 인스턴스는 인터넷에 바로 아웃바운드 트래픽을 전송할 수 있는 반면, 프라이빗 서브넷의 인스턴스는 그렇게 할 수 없습니다. 

반면, 프라이빗 서브넷의 인스턴스는 퍼블릭 서브넷에 있는 NAT(Network Address Translation) 게이트웨이를 사용하여 인터넷에 액세스할 수 있습니다. 

AWS는 VPC의 보안을 강화하기 위해 사용할 수 있는 두 가지 기능인 보안 그룹과 네트워크 ACL을 제공합니다. 

보안 그룹은 인스턴스용 인바운드 및 아웃바운드 트래픽을 제어하고, 네트워크 ACL은 서브넷용 인바운드 및 아웃바운드 트래픽을 제어합니다.

## 참고

CloudTrail은 사용장 활동 및 API 사용추적->API 사용추적을 통해 보안 분석 및 문제 해결을

VPC 흐름 로그 -> IP 트래픽에 대한 정보를 수집할 수 있는 기능이다.

Amazon CloudWatch ->애플리케이션 모니터링 사용량 지표,이벤트 운영 데이터 수집을 목표로함.

## 관련 문제

### NO.167 
A company has an AWS environment that consists of a VPC. multiple subnets, and many Amazon EC2 instances in the subnets An engineer wants to restrict inbound traffic to one particular EC2 instance without affecting the other EC2 instances.

A. Network ACLs

### NO.249 
Which AWS feature or service can be used to capture information about incoming and outgoing traffic in an AWS VPC infrastructure?

-> VPC Flow Logs

### NO.283 
Which AWS service or component allows inbound traffic from the internet to access a VPC?

-> NAT gateway
