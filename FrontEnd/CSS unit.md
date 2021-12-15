# CSS Unit

## 

## CSS의 표준권고안에 따르면 크기 단위는 절대 단위와 상위 단위로 구분됨.

* ### 절대 단위(Absolute unit) : 절대 단위는 크기가 고정되어 있어 이들 중 하나로 표시된 길이는 정확히 그 크기로 나타난다. 화면의 크기는 매우 다양하기 때문에 절대 길이 단위는 화면에서 사용하지 않는 것이 좋다. 단, **출력 매체를 알고있는 경우 효율적으로 사용할 수 있다.**

  * cm : 센티미터다.
  * mm : 밀리미터, cm의 1/10이다.
  * in(인치) : 1in은 2.54cm이다.
  * pt(포인트) : 1pt는 1/72 in 이며 문자 크기를 지정할 때 사용한다.
  * pc:(파이커) : 1pc는 12pt이다.

* ### 상대 단위(Relative unit) : 플랫폼, 기종 간의 호환성을 유지하는데 유리하다. 다른 요소나 창 크기에 비례하여 크기가 조정되기 때문에 반응형 사이트의 스타일을 지정하는데 유용하다.

  * px : 픽셀(pixel), 해상도에 따라 달라진다. 
  * % : 브라우저 기본 글꼴 크기를 100%로 하고 상대적 크기를 나타낸다.
  * em : 브라우저 기본 글꼴 크기를 1em으로 하고 상대적 크기를 나타낸다.
  * ex : 소문자 x의 높이를 기준으로 한다.

reference : 

> https://zinee-world.tistory.com/131
>
> jae04099.tistory.com/entry/CSS-반응형-단위-정리vh-em-rem-등
>
> https://developer.mozilla.org/ko/docs/Learn/CSS/Building_blocks/Values_and_units
>
> https://mainia.tistory.com/3894
>
> http://daplus.net/css-css-ex단위의-가치는-무엇입니까/
>
> **📌 : 자료 찾는데 각 자료마다 다른 부분이 많아 틀린 곳 있을 수 있습니다. 오류 지적 환영 📌**



