# Git_flow & Github_flow 알아보기



### Git_flow

아래는 Git_flow를 설명할 때 유용한 사진이다.

![git-flow_overall_graph](https://techblog.woowahan.com/wp-content/uploads/img/2017-10-30/git-flow_overall_graph.png)

#### Git flow는 5가지 브런치를 사용한다.

* main(=master) : **master보다는 main이라는 이름**으로 더 많이 사용 중이다. 프로젝트 시작부터 끝까지 유지되는 메인 브런치이다.
  * 개발을 다 끝내고 제품으로 출시할 수 있을 때 이용하는 브런치다.
* develop : main 브런치와 함께 끝까지 유지되는 메인 브런치로, 다음 출시 버전을 개발하는 브런치다.
  * 참고로 위 사진에서 볼 수 있듯이 main 브런치보다 develop 브런치가 좀 더 활발히 이용된다.
* feature : 직접적으로 기능을 개발하는 브런치이며 다수의 브런치를 만들 수 있다. 여러번 만들어지고 사라지는 보조 브런치다.
  * 팀프로젝트에서 여러 feature 브런치를 만들어 각자 개발을 하고 develop 브런치로 넘기거나,
    혼자서 여러 부분을 개발하며 브런치를 늘릴 수 있다.
  * 필자 생각에 프로젝트를 진행하며 가장 많이 사용하는 브런치이다. 개인적으로 feature 브런치를 이용해
    세밀하게 개발 부분을 나눠 정리하면 매우 좋을것이라 본다.
* release : develop에서 개발한 것들을 main 브런치로 넘길 때 사용된다. 보조 브런치다.
  * 보통 feature 브런치에서 남겼던 주석을 지우고 main으로 넘긴다.
    * 필자는 release 이름을 [SemVer 방식](https://github.com/dsmjimin/TIL-MD/blob/main/Node.js%20Package%20Version.md)으로  정한다.
* hotfix : 출시 버전에서 출시 버전에서 발생한 버그를 수정하기 위해 만든다. 보조 브런치이다.
  * 필자는 아직까지 사용해 본 적이 없지만, 생각을 얘기해보자면 지속적으로 유지보수를 하는 프로젝트에 주로 사용할듯하다.

### Github_flow

![Git TextBook | 깃브랜치&gt;전략](https://git.jiny.dev/gitflow/img/gitflow_02.png)

release : 

> https://techblog.woowahan.com/2553/

📢 Git_flow branch 설명 부분 제외 혼자 작성 중.

📢 오타, 오류 지적 환영!
