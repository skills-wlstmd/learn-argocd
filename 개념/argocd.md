# ArgoCD

- GitOps continuous delivery tool for k8s
- GitOps방식으로 관리되는 Manifest 파일의 변경사항을 감시하며 현재 배포된 환경의 상태와 Git에 정의된 Manifest 상태를 동일하게 유지
- push / pull 타입 모두 지원하며 pull 타입 배포를 권장
- GitOps
  - 위브웍스(Weaveworks)에서 처음 사용한 프로젝트에 DevOps를 적용하는 용어
  - Cloud Native + k8s대상의 Continuous Deployment에 초점

`ArgoCD 문제점`

- k8s에서만 사용가능
- on-premise, AWS SaaS(ex. Elastic Beanstalk)환경에서 사용 불가능
- git 서비스 장애 : 새로운 업데이트 반영 X
  - github(public)
  - self-managed
