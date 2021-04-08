## [Elastic Load Balancing (ELB)](https://docs.aws.amazon.com/ko_kr/elasticloadbalancing/latest/userguide/load-balancer-getting-started.html)

Elastic Load Balancing은(는) 둘 이상의 가용 영역에서 EC2 인스턴스, 컨테이너, IP 주소 등 여러 대상에 걸쳐 수신되는 트래픽을 **자동으로 분산**합니다.

## 로드 밸런서 유형

   * [Application Load Balancer](#Application-Load-Balancer)
   * [Network Load Balancer](#Network-Load-Balancer)
   * [Gateway Load Balancers](#Gateway-Load-Balancers)
   * [Classic Load Balancer](#Classic-Load-Balancer)

Amazon ECS 서비스는 어느 유형의 로드 밸런서든 사용할 수 있습니다.

Application Load Balancer는 HTTP/HTTPS (또는 Layer 7) 트래픽을 라우팅할 때 사용됩니다. Network Load Balancer 및 Classic Load Balancer는 TCP(또는 Layer 4) 트래픽을 라우팅할 때 사용됩니다.

## Application Load Balancer

Application Load Balancer는 개방형 시스템 간 상호 연결(OSI) 모델의 일곱 번째 계층인 애플리케이션 계층에서 작동합니다.

## Network Load Balancer

Network Load Balancer는 개방형 시스템 간 상호 연결(OSI) 모델의 네 번째 계층에서 작동합니다. 

## Gateway Load Balancers

게이트웨이 로드 밸런서를 사용하면 방화벽, 침입 탐지 및 방지 시스템, 심층 패킷 검사 시스템 같은 가상 어플라이언스를 배포, 확장 및 관리할 수 있습니다.

게이트웨이 로드 Load Balancer 개방형 시스템 간 상호 연결(OSI) 모델의 세 번째 계층인 네트워크 계층에서 작동합니다.

## Classic Load Balancer

로드 밸런서는 수신 애플리케이션 트래픽을 여러 가용 영역의 여러 EC2 인스턴스에 분산합니다.

