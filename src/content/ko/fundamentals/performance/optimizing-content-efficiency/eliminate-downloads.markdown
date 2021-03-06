---
title: "불필요한 다운로드 제거하기"
updated_on: 2014-04-29
translators:
  - captainpangyo
key-takeaways:
  eliminate-downloads:
    - "페이지의 모든 자원 및 3rd 파티 자원 목록 만들어 관리하기"
    - "각 자원의 성능을 측정하기: 그 가치와 기술적인 성능"
    - "그 자원이 충분한 가치를 제공하는지 확인하기"
---

<p class="intro">
가장 빠르고 최적화가 잘되어 있는 자원은 전송되지 않은 자원이다. 당신의 자원을 최근에 점검해보셨나요? 각 자원이 보다 나은 사용자 경험을 돕고 있는지 확인하기 위해 자원을 주기적을 점검하셔야 합니다.
</p>

{% include shared/takeaway.liquid list=page.key-takeaways.eliminate-downloads %}

가장 빠르고 최적화가 잘되어 있는 자원은 전송되지 않은 자원입니다. 물론, 이 말이 당연한 것처럼 보일지 몰라도, 실제로 이 것이 자주 간과됩니다: 성능 엔지니어로서, 당신의 어플리케이션에서 불필요한 자원들을 제거할 수 있는 기회를 보는 눈을 길러야 합니다. 당신의 팀원들에게 질문하고, 정기적으로 재 방문하고, 명시적 묵시적 추측을 갖는 것이 중요한 연습이 됩니다. 몇 가지 예제를 봅시다 :

* 우리는 X 자원을 페이지에 항상 포함시켜왔습니다, 하지만 이 자원을 다운로딩하고 화면에 표시하는 비용이 사용자에게 보여질만한 가치를 합니까? 우리가 이 것을 측정할 수 있고 그 가치를 증명할 수 있습니까?
* 이 자원이 &mdash; 특히 만약 이 자원이 3rd 파티 자원인 경우 &mdash; 일정한 성능을 제공하는가요? 이 자원이 크리티컬 패스에 포함되는 것인가요? 아니면 있어야 하는 것인가요? 만약 그 자원이 크리티컬 패스에 있다면, 그 것이 우리 사이트 실패의 원인이 될 수 있는가요? - 혹은 자원이 이용 불가능 하다면, 그 것이 성능 전체나 페이지 사용자 경험에 영향을 미칠 것인가요?
* 이 자원이 SLA 가져야 하거나 필요한가? 이 자원은 성능 모범 사례를 따르는가: 압축, 캐싱, 등등?

너무나 빈번하게 우리의 페이지들이 불필요한 자원을 포함하거나 혹은 더 안좋게는, 사이트나 사용자에게 많은 가치를 제공하지도 않으면서 페이지 성능을 가로막는 요소가 됩니다. 이 것이 1rd 파티와 3rd 파티자원과 위젯에 동일하게 적용됩니다.

* Site A 는 방문자들이 여러 사진을 빠르게 클릭할 수 있도록 사진 회전 기능을 홈페이지에 표시하기로 결정하였습니다 &mdash; 모든 사진들은 페이지가 로딩 되었을 때, 로딩되어야 하고 사용자들에 의해 실행됩니다.
    * **질문:** 얼마나 많은 사용자들이 사진회전 기능 안의 사진들을 보는 지 측정한 적이 있습니까? 대부분의 사용자들이 보지도 않는 불필요한 자원들을 다운 받음으로써 높은 오버헤드가 발생할 수 있습니다.
* Site B 는 연관된 소셜 컨텐츠를 표시하고 다른 서비스를 제공하기 위해 3rd 파티 위젯을 설치하기로 결정했습니다.
    * **질문:** 얼마나 많은 방문자들이 이 위젯을 사용하는지? 또는 그 위젯에서 제공하는 컨텐츠가 얼마나 클릭 되는지 측정 해본적이 있습니까? 이 위젯에 의해 생성된 효과가 그 오버헤드를 감당할 만한 이유가 있나요?

이처럼, 불필요한 다운로드를 제거하는 것이 매우 흔한 일인 것처럼 보이지만, 실제로는 그 것이 종종 구현되어야 하는 이유를 많이 생각해보게 하고, 측정을 요하게 하는 일입니다. 사실 최상의 결과를 위해서는 주기적으로 목록을 관리하고, 페이지의 모든 자원들에 대해 각각 이 질문들을 해봐야 합니다.
