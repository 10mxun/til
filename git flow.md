# Git Flow
<hr>
## Git Flow는
- Vincent Driessen이 제안한 Git 브랜칭 모델로, 대규모 프로젝트나 주기적인 릴리즈가 필요한 환경에서 체계적이고 구조적인 개발 프로세스를 제공한다.
- master, develop, feature, release, hotfix 5가지 브랜치를 사용하여 기능 개발, 배포, 유지보수를 철저히 분리하여 관리한다
<hr>
## 주요 브랜치 구조
- master (main) : 항상 프로덕션 환경에 **배포 가능한 상태를 유지**하는 브랜치
- develop : 다음 버전을 위해 개발 중인 코드가 모이는 **메인 브랜치**
<hr>
## 보조 브랜치 구조
- feature : **새로운 기능 개발 시 develop 브랜치에서 분기**하며, 개발 완료 후 develop으로 병합된다
- release : **배포 준비**를 위한 브랜치이며, develop 브랜치에서 분기하여 QA 및 버그 수정을 수행 후 master 브랜치와 develop 브랜치로 병합된다
- hotfix : 배포된 master 버전에서 **긴급한 버그가 발생**했을 때 사용하며, 즉시 수정 후 master와 develop에 반영한다.
<hr>
## Git Flow의 장단점
<hr>
- [x] 장점
  - 엄격한 규칙을 통해 대규모 협업에서 코드 충돌을 줄이고, 구조화된 배포 프로세스를 제공한다
- [ ] 단점
  -  구조가 복잡하여 소규모 프로젝트에는 오버엔지니어링이 될 수 있으며, 브랜치 전환 및 병합이 잦다.
<hr>
## Git FLow 시나리오
<hr>
[Image] : https://devocean.sk.com/editorImg/2024/8/21/6e8114c0510c505512467f476426cc89303e0de5cdd5dc1c9e95d6e3bc538f62


