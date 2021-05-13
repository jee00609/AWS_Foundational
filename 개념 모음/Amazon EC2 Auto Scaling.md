## [Amazon EC2 Auto Scaling](https://docs.aws.amazon.com/ko_kr/autoscaling/ec2/userguide/what-is-amazon-ec2-auto-scaling.html)

Amazon EC2 Auto Scaling를 통해 애플리케이션의 로드를 처리할 수 있는 정확한 수의 Amazon EC2 인스턴스를 보유하도록 보장할 수 있습니다.

## Amazon EC2 Auto Scaling 장점

   * **내결함성 향상**
      * Amazon EC2 Auto Scaling에서는 인스턴스가 비정상 상태일 때 이를 감지하여 종료한 다음 이를 대체할 인스턴스를 시작할 수 있습니다. 
      * 여러 개의 가용 영역을 사용하도록 Amazon EC2 Auto Scaling을 구성할 수도 있습니다. 
      * 하나의 가용 영역이 사용 불가 상태가 되면 Amazon EC2 Auto Scaling에서는 다른 가용 영역에서 새 인스턴스를 시작하여 이에 대처할 수 있습니다.
   * **가용성 향상**
      * Amazon EC2 Auto Scaling은 애플리케이션이 항상 현재 트래픽 요구를 처리할 수 있는 올바른 용량을 갖추도록 도와줍니다.
   * **비용 관리 개선**
      * Amazon EC2 Auto Scaling는 필요에 따라 **용량을 동적으로 확장 및 축소**할 수 있습니다. 
      * 사용한 EC2 인스턴스에 대해서만 비용을 지불하므로, 인스턴스가 필요할 때 이를 시작하고 필요 없어지면 종료함으로써 비용을 절감합니다.

## 관련 문제

### NO.236 
A company wants to focus on business activities instead of managing compute and capacity Which AWS service can be used to automatically add or remove Amazon EC2 instances based on-demand)

-> Amazon EC2 Auto Scaling
