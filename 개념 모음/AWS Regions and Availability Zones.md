## [Regions and Availability Zones](https://aws.amazon.com/about-aws/global-infrastructure/regions_az/?nc1=h_ls)

## 리전

AWS가 전 세계에서 **데이터 센터를 클러스터링하는 물리적 위치를 리전**이라고 합니다.

**논리적 데이터 센터의 각 그룹을 가용 영역**이라고 합니다.

각 AWS **리전은 지리적 영역 내에서 격리되고 물리적으로 분리된 여러 개의 AZ로 구성**됩니다.

각 AZ는 독립된 전원, 냉각 및 물리적 보안을 갖추고 있으며 지연 시간이 매우 짧은 중복 네트워크를 통해 연결됩니다. 

고가용성을 중시하는 AWS 고객은 여러 AZ에서 실행되도록 애플리케이션을 설계하여 내결함성을 한층 더 강화할 수 있습니다. 

AWS 인프라 리전은 가장 높은 수준의 보안, 규정 준수 및 데이터 보호를 충족합니다.

## 가용 영역

AZ(가용 영역)는 AWS 리전의 중복 전력, 네트워킹 및 연결이 제공되는 하나 이상의 개별 데이터 센터로 구성됩니다. 

AZ를 사용하면 단일 데이터 센터를 사용하는 것보다 **더 높은 가용성, 내결함성 및 확장성을 갖춘 프로덕션 애플리케이션과 데이터베이스를 운영**할 수 있습니다.

AWS 리전의 모든 AZ는 **높은 대역폭, 지연 시간이 짧은 네트워킹, 완전한 중복성을 갖춘 전용 메트로 광 네트워크와 상호 연결**되어 있어 AZ 간에 **높은 처리량과 지연 시간이 짧은 네트워킹**을 제공합니다.

AZ 간의 **모든 트래픽은 암호화**됩니다. 

네트워크 성능은 AZ 간 **동기 복제 기능을 충분히 수행**할 수 있습니다. 

AZ는 **고가용성을 위한 애플리케이션 분할을 용이**하게 합니다. 

애플리케이션 하나를 여러 AZ에 걸쳐 분할하면 기업의 격리가 더 원활하게 이루어지며 정전, 낙뢰, 토네이도, 지진 등과 같은 문제로부터 안전하게 보호됩니다. 

AZ는 다른 모든 AZ와 수 킬로미터에 상당하는 **유의미한 거리를 두고 물리적으로 분리**되어 있습니다.

## 연속성 향상
AZ를 사용하여 같은 리전 내의 여러 데이터 센터에 애플리케이션과 데이터를 복제하는 것과 더불어, **AWS 리전 간에 데이터를 복제함으로써 중복성과 내결함성도 향상할 수 있습니다. **

프라이빗 고속 네트워킹 및 퍼블릭 인터넷 연결 모두를 사용하여 비즈니스 연속성에 계층을 추가하거나 전 세계적으로 지연 시간이 짧은 액세스를 제공할 수 있습니다.

## 관련 문제

### NO.242 
Which AWS feature should a customer leverage to achieve high availability of an application?

-> Availability Zones

### NO.260 ()
When a company provisions web servers in multiple AWS Regions, what is being increased?

-> Durability(내구성) OR  Availability(가용성)

-> 내구성은 데이터가 유실되지 않는 것을 뜻하며 가용성은 언제나 정상적으로 사용 가능한 상태를 

#### NO.261 
Which statement is true about AWS global infrastructure?

-> AWS Regions consist of multiple Availability Zones.

## NO.294 
A cloud practitioner is developing a disaster recovery plan and intends to replicate data between multiple geographic areas. <br/>
Which of the following meets these requirements?

-> AWS Regions
