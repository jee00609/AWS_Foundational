## [AWS Global Accelerator](https://docs.aws.amazon.com/ko_kr/global-accelerator/latest/dg/what-is-global-accelerator.html)

AWS Global Accelerator는 **전 세계 사용자가 사용하는 인터넷 애플리케이션의 가용성과 성능을 개선**하기 위해 액셀러레이터를 생성하는 네트워크 계층 서비스

AWS Global Accelerator 는 사용자가 액셀러레이터 로컬 및 글로벌 사용자를 위해 **애플리케이션의 가용성과 성능을 개선**합니다. 

AWS Global Accelerator는 로컬 및 글로벌 사용자의 애플리케이션 성능을 개선하기 위해 액셀러레이터 를 생성하는 서비스입니다. 

선택한 액셀러레이터 유형에 따라 추가 혜택을받을 수 있습니다.

   * 표준 가속기를 사용하면 전 세계 사용자가 사용하는 인터넷 응용 프로그램의 가용성을 향상시킬 수 있습니다.<br/> 표준 가속기를 사용하는 Global Accelerator는 AWS 글로벌 네트워크를 통해 클라이언트에 가장 가까운 리전의 엔드 포인트로 트래픽을 보냅니다.
   * 사용자 지정 라우팅 가속기를 사용하면 한 명 이상의 사용자를 여러 대상 사이의 특정 대상에 매핑 할 수 있습니다.

## 단일 리전 애플리케이션의 지연 시간 및 가용성 개선

AWS Global Accelerator는 로컬 및 글로벌 트래픽의 네트워크 라우팅을 개선하므로 단일 리전 배포와 다중 리전 배포 간의 차이를 줄이는 데 도움이 됩니다.

Global Accelerator를 사용하면 사용자 트래픽이 80개 이상의 글로벌 엣지 로케이션을 통해 인터넷에서 Amazon의 프라이빗 글로벌 네트워크로 이동한 다음 애플리케이션 오리진으로 연결됩니다.

AWS Global Accelerator는 설정이 빠르며 트래픽 성능을 최대 60% 개선합니다.

## 관련 문제

### NO.201 
Which AWS services help to improve application performance by reducing latency while accessing content globally? (Select TWO.)

### NO.246 
A company is planning to launch an ecommerce site in a single AWS Region to a worldwide user base Which AWS services will allow the company to reach users and provide low latency and high transfer speeds? (Select TWO)

-> **AWS Global Accelerator** & **Amazon CloudFront**
