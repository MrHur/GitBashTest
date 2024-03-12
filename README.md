# GitBashTest

Git_bash_test Repository입니다.

이 저장소는 CLI 에 익숙해지고, Git or Git_bash를 숙달하기 위해 만들어졌습니다.

Git_bash를 쓰는 이유는 Linux 환경에 익숙해지기 위해서입니다.


![3c38e8](https://github.com/MrHur/GitBashTest/assets/79696786/dbd78d9a-6411-4f6a-9920-2f9c486bf76d)

<Git bash 기본 명령어>

여기에 몇 가지 기본적인 Git 명령어를 제공합니다. 이러한 명령어들은 Git을 사용하여 프로젝트를 관리하고 버전을 관리하는 데 도움이 됩니다:

git init: 현재 디렉토리를 Git 저장소로 초기화합니다.

git clone [url]: 원격 저장소의 프로젝트를 복제합니다.

git add [file]: 변경된 파일을 Staging Area에 추가합니다.

git commit -m "[message]": Staging Area에 있는 변경 사항을 커밋합니다.

git status: 현재 작업 디렉토리의 상태를 확인합니다.

git log: 커밋 기록을 조회합니다.

git pull: 원격 저장소에서 최신 변경 사항을 가져와 현재 브랜치에 병합합니다.

git push: 현재 브랜치의 변경 사항을 원격 저장소로 푸시합니다.

git branch: 브랜치 목록을 표시합니다.

git checkout [branch_name]: 특정 브랜치로 전환합니다.

git merge [branch_name]: 다른 브랜치를 현재 브랜치에 병합합니다.

git remote -v: 현재 연결된 원격 저장소를 확인합니다.

git remote add [name] [url]: 새로운 원격 저장소를 추가합니다.

git remote remove [name]: 원격 저장소를 제거합니다.

git diff: 변경된 내용을 확인합니다.

---


GIT을 능숙하게 다루기 위해서는 다음과 같은 항목을 학습하고 연습하는 것이 도움이 됩니다:

기본 개념 이해:

버전 관리 시스템의 기본 개념과 GIT의 작동 방식을 이해합니다.
커밋, 브랜치, 병합, 리베이스, 충돌 해결 등의 핵심 개념을 숙지합니다.
GIT 명령어 숙지:

기본적인 GIT 명령어인 clone, init, add, commit, push, pull, fetch, merge, rebase, checkout, branch 등을 익힙니다.
GIT 명령어의 옵션과 사용법을 익숙하게 합니다.
브랜치 전략 이해:

효율적인 협업을 위한 다양한 브랜치 전략을 이해하고 적용하는 방법을 배웁니다. 예를 들어, Gitflow, Feature Branch, Forking Workflow 등이 있습니다.
충돌 해결 및 리베이스:

여러 명이 협업할 때 발생하는 충돌을 해결하는 방법을 익히고, 리베이스를 사용하여 커밋 히스토리를 정리하는 방법을 익힙니다.
GIT 원리 이해:

GIT의 내부 동작 원리를 이해하여 문제가 발생했을 때 빠르게 해결할 수 있는 능력을 기릅니다.
코드 리뷰 및 협업 도구:

Pull Request를 통한 코드 리뷰와 협업을 이해하고, 협업 도구를 사용하는 방법을 익힙니다. (예: GitHub, GitLab, Bitbucket 등)
보안 및 권한 관리:

GIT 저장소의 보안과 권한 관리에 대한 이해와 사용법을 학습합니다.
실전 연습:

프로젝트를 진행하면서 GIT을 사용하여 실전 경험을 쌓습니다. 버전 관리와 협업을 위해 GIT을 활용하는 프로젝트를 진행합니다.
오픈 소스 프로젝트 참여:

오픈 소스 프로젝트에 참여하여 다른 사람들과의 협업을 경험하고, 다양한 GIT 사용 사례를 익힙니다.
GIT을 능숙하게 다루기 위해서는 이러한 항목들을 숙지하고 연습하는 것이 중요합니다. 지속적인 학습과 실전 경험을 통해 GIT 사용 능력을 향상시킬 수 있습니다.

---

GIT Branch 전략
<br>
Gitflow, Feature Branch, Forking Workflow는 Git을 사용하여 소프트웨어 개발을 위한 다양한 브랜치 전략입니다. 각각의 전략은 프로젝트의 규모, 팀 구성 및 개발 프로세스에 맞게 선택할 수 있습니다.
<br>

Gitflow는 Vincent Driessen에 의해 제안된 브랜치 관리 전략입니다. <br>
주요 특징은 다음과 같습니다: <br>
<br>
Master 브랜치: 제품 출시 버전을 관리하는 메인 브랜치입니다. 안정적인 상태의 코드만을 유지합니다. <br>
Develop 브랜치: 다음 출시를 위한 개발이 진행되는 브랜치입니다. 개발이 완료되면 Master 브랜치로 병합됩니다. <br>
Feature 브랜치: 새로운 기능을 개발하기 위한 브랜치입니다. Develop 브랜치에서 분기되고, 기능이 완료되면 Develop 브랜치로 병합됩니다. <br>
Release 브랜치: 새로운 출시를 준비하는 브랜치입니다. Develop 브랜치에서 분기되고, 품질 검증이 완료된 후 Master 브랜치와 Develop 브랜치로 병합됩니다. <br>
Hotfix 브랜치: 제품의 긴급한 버그 수정을 위한 브랜치입니다. Master 브랜치에서 분기되고, 수정이 완료되면 Master와 Develop 브랜치로 병합됩니다. <br>

Feature Branch 전략은 각각의 기능을 별도의 브랜치로 관리하는 전략입니다. <br>
주요 특징은 다음과 같습니다: <br>
<br>
각각의 기능은 Develop 브랜치에서 분기된 별도의 브랜치로 개발됩니다. <br>
기능 개발이 완료되면 Develop 브랜치로 다시 병합됩니다. <br>
이러한 방식으로 기능 간 충돌이 최소화되고, 개발 과정을 보다 모듈화하고 추적하기 쉽습니다. <br>

  
Forking Workflow는 각 개발자가 자신의 개인 저장소에서 작업을 수행하는 전략입니다. <br>
주요 특징은 다음과 같습니다: <br>
<br>
프로젝트 저장소를 개인 계정으로 Fork하여 개인 작업을 수행합니다. <br>
개인 저장소에서 변경 사항을 커밋하고, 원본 프로젝트 저장소로 Pull Request를 보냅니다. <br>
팀의 다른 구성원이 Pull Request를 검토하고 승인하면 변경 사항이 원본 프로젝트에 병합됩니다. <br>
각각의 브랜치 전략은 프로젝트의 요구 사항과 팀 구성에 따라 선택되어야 합니다. 개발자와 팀은 이러한 전략 중 가장 적합한 것을 선택하고, 일관된 개발 프로세스를 유지하면서 효율적으로 협업할 수 있습니다. <br>

---

<reference>

  출처 : http://osteele.com
