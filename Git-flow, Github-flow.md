# Git-flow , Github-flow 간단하게 살펴보기

**Git-flow 전략은 소프트웨어의 소스코드를 관리하고 출시하기 위한 '브랜칭 관리 전략(branch management strategy)'이 있다.**

**ㅡ 이 전략의 단점을 극복하기 위해 Github flow와 Gitlab flow 전략이 나왔다.**

**Git-flow에는 5가지 종류의 브랜치가 있다.**

**항상 유지되는 메인 브랜치들(main, develotp)과 일정 기간 동안만 유지되는 보조 브랜치들(feature, release, hotfix)이 있다.**

###### § feature > develop > release > hotfixes > main 순서로 진행된다. §

* **main : 제품으로 출시될 수 있는 브랜치(배포)**

* **develop : 다음 출시 버전을 개발하는 브랜치(개발)**

* **feature : 기능을 개발하는 브랜치(기능)**

* **release : 이번 출시 버전을 준비하는 브랜치(출시)**

* ##### **hotfix : 출시 버전에서 발생한 버그를 수정하는 브랜치(긴급수정)**

![git-flow_overall_graph](https://techblog.woowahan.com/wp-content/uploads/img/2017-10-30/git-flow_overall_graph.png)

* #### 장점

  * #### 명령어가 나와있다.

  * #### 웬만한 에디터와 IDE에는 플러그인으로 존재한다.

* #### 단점

  * #### 브런치가 많아 복잡하다.

  * #### 안쓰는 브런치, 쓰기 애매한 브런치가 존재한다.



# Github-flow

**Git-flow도 좋은 방식이지만 Github에 적용하기엔 복잡하다는 Scott Chacon의 판단에 따라 만들어진 새로운 깃 관리 방식.**

**자동화 개념이 들어가있으며, 자동화가 적용되어 있지 않은 곳은 수동으로 진행한다.**

**Git-flow에 비해 흐름이 단순해짐에 따라 규칙 또한 단순해졌다.**

**피드백이나 도움이 필요할 때, 그리고 병합(merging) 준비가 완료되었을 때는 pull request를 생성한다.**

* #### 장점

  * 브런치 전략이 단순하다.
  * Github 사이트에서 제공하는 기능을 모두 사용하여 작업을 진행한다.
  * CI가 필수적이며, 배포는 자동으로 진행 가능하다.

* #### 단점

  * CI와 배포 자동화가 되어있지 않은 시스템에서는 사람이 해당 업무를 진행해야 한다.
  * 프로젝트의 규모가 커짐에 따라 점점 관리에 어려움이 발생할 수 있다.



reference

https://gist.github.com/ihoneymon/a28138ee5309c73e94f9

https://techblog.woowahan.com/2553/

https://ujuc.github.io/2015/12/16/git-flow-github-flow-gitlab-flow/

https://codingtrainee.tistory.com/156

https://k39335.tistory.com/82

