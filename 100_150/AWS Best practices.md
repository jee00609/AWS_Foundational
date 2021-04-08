## Best practices(모범 사례)

AWS 모범 사례는 무엇입니까?

   * [사용자에 대해 AWS MFA (AWS Multi-Factor Authentication)를 활성화합니다.](https://docs.aws.amazon.com/ko_kr/organizations/latest/userguide/best-practices_member-acct.html#best-practices_mbr-acct_mfa)
   * [사용자를위한 강력한 암호 정책을 구성하십시오.](https://docs.aws.amazon.com/ko_kr/IAM/latest/UserGuide/id_credentials_passwords_account-policy.html)

AWS 모범 사례가 아닌 것은?
   * ~~사용자 관리 형 정책 대신 인라인 정책을 사용하십시오.~~ 
      * [인라인 정책 대신 고객 관리형 정책을 사용하는 것이 가장 좋습니다.](https://aws.amazon.com/ko/premiumsupport/knowledge-center/iam-increase-policy-size/)
   * ~~~자격 증명을 교체하지 마십시오.~~
      * [자격 증명을 정기적으로 교체](https://docs.aws.amazon.com/ko_kr/IAM/latest/UserGuide/best-practices.html)
   * ~~사용자 간 액세스 키 공유를 활성화합니다~~
      * [다른 사람과 AWS 계정 루트 사용자 암호 또는 액세스 키를 공유하지 마십시오. ](https://docs.aws.amazon.com/ko_kr/IAM/latest/UserGuide/best-practices.html)
