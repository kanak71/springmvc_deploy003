Github Actions

1. Github Actions 사용

 - 비밀번호를 코드에 입력하는 방식이 아니라 Github Screte Key 를 만들어서 값을 코드 입력하겠다
   
 - Gihub Actions은 workflow(Pipe line)을 통해서 단계별로 작성한다
    - workflow의 의미는 단계로 되어 있다. 따라서 중간에 멈추거나 문제가 발생하면 쉽게 고칠 수 있다
    - 단계별로 먼저 실행을 한 후에 최종 동작을 만들어 낼 수 있다

  - workflow를 작성한다

## Git push만 하면 자동으로 Maven 빌드하고 Tomcat에 배포되는 자동 배포 시스템 만든 것




1) Webhook(springMVC_deploy001에서 한 것)
### GitHub가 다른 서버를 깨우는 알림 장치

    - GitHub에서 이벤트 발생하면 (push, PR 등)
    지정한 URL로 HTTP 요청 날림
    예: Jenkins, 서버, Discord 등

2) GitHub Actions (현재 repository)

### GitHub 안에서 아예 자동으로 다 실행하는 공장

  - push 발생
  GitHub 서버가 직접
  코드 가져오고
  Maven 빌드하고
  테스트하고
  배포

  - GitHub 자체가 CI/CD 실행 환경
   - 서버 따로 없어도 됨
   - workflow(yml)로 “자동화 설계도” 작성
