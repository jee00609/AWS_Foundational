## [Setting an account password policy for IAM users](https://docs.aws.amazon.com/IAM/latest/UserGuide/id_credentials_passwords_account-policy.html)

## 암호 관리

AWS 계정 루트 사용자 및 계정의 IAM 사용자의 암호를 관리할 수 있습니다. 

IAM 사용자가 AWS Management 콘솔에 액세스하려면 암호가 필요합니다. 

사용자가 AWS CLI, Windows PowerShell용 도구, AWS SDK 또는 API를 사용하여 프로그래밍 방식으로 AWS 리소스에 액세스하는 경우 암호가 필요 없습니다. 

대신 그러한 환경에서는 사용자에게 액세스 키가 필요합니다

## IAM 사용자의 계정 암호 정책 설정

AWS 계정에서 사용자 지정 암호 정책을 설정하여 IAM 사용자 암호의 복잡성 요건과 의무적인 교체 주기를 지정할 수 있습니다.

사용자 지정 암호 정책을 설정하지 않은 경우 IAM 사용자 암호는 기본 AWS 암호 정책을 충족해야 합니다.

사용자 지정 암호 정책 옵션

계정에 대한 사용자 지정 암호 정책을 구성할 때 다음 조건을 지정할 수 있습니다.

## 사용자 지정 암호 정책 옵션

   * 암호 최소 길이
   * 암호 강도
   * 암호 만료 활성화
   * 암호 만료 시 관리자 재설정 필요
   * 사용자 자신의 암호 변경 허용
   * 암호 재사용 제한

## AWS에서 Multi-Factor Authentication(MFA) 사용

보안 강화를 위해 멀티 팩터 인증(MFA)을 구성하여 AWS 리소스를 보호하는 것이 좋습니다. 

IAM 사용자 또는 AWS 계정 루트 사용자에 대해 MFA를 활성화할 수 있습니다. 

루트 사용자에 대해 MFA를 활성화하면 해당 루트 사용자 자격 증명에만 적용됩니다. 

이 계정의 IAM 사용자들은 자신의 자격 증명에 더하여 별도로 자격 증명을 갖게 되며, 이 별도의 자격 증명에 고유의 MFA가 구성됩니다.

## 관련 문제

### NO.256 
AWS supports which of the following methods to add security to Identity and Access Management (IAM) users? (Select TWO.)

-> **Using Multi-Factor Authentication (MFA)** & **Enforcing password strength and expiration**
