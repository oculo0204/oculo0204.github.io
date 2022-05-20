## 0\. css란

css란 cascading style sheet의 약자로

html 요소들이 각종 미디어에서 어떻게 보이는가를 정의하는 데 사용하는 스타일 시트 언어입니다.

css를 사용하는데 가장 큰 장점은 스타일을 저장하는 파일을 따로 만들 수 있다는 것입니다. (물론, inline, internal, external방식 중 external에 해당됨) 이렇게 하면 html요소의 스타일을 html요소 내부에서 일일이 지정할 필요없이 스타일만 따로 제어할 수 있습니다. 스타일의 변경 및 유지보수가 쉬워집니다.

주의할 것은 css는 html문법을 따르지 않는다는 것입니다.

예를 들어

|       html   <h1 style="color:blue">         css   h1{ color : blue }          |
| --- |

주석 또한 다릅니다. 

|       html   <!-- 뭐시기 뭐시기 어쩌라고 -->      css   /\* 뭐시기 뭐시기 어쩌라고 \*/          |
| --- |
<br><br><br>
## 1.  cascading 

css는 "cascading" style sheet의 줄임말로 script 형식의 언어인 html에서 사용할 수 있는 " 중첩하고 상속할 수 있는" style을 말합니다. 오늘은 이러한 css의 특성을 이용할 수 있게 해주는 선택자와 그 우선순위에 대해 알아보도록 하겠습니다.

---

## 2\. 구체적인 사용자 정의 스타일 >> 좀 더 큰 범위의 사용자 정의 스타일 >> 브라우저 기본값

cascading의 특징

앞서 말했던 것처럼 css는 계층적인 구조가 가능한 stylesheet입니다. 이러한 형식을 통해 우리는 전체적인 그림을 그리고 나서 작고 세부적인 것을 채워나갈 수 있습니다. css는 큰 스타일을 지정하고 작은 스타일들을 적용하기 때문에 <정의된 세부 스타일이 있다면 그것을 먼저 사용하고 그 다음에 좀 더 큰 정의, 더 큰 정의를 사용합니다.> 그렇기 때문에 사용자가 정의한 스타일이 우선적으로 적용되고 그러고도 정의되지 않은 것이 있다면 브라우저에서 기본으로 정의해놓은 값을 사용합니다.

cascading의 우선순위

Author Style(개발자가 지정한 것) >> User Style(사용자가 지정한 것) >> Browser Style

---

다음 시간에는 선택자와 우선순위에 대해 본격적으로 알아보도록 하겠습니다.
<br><br><br><br><br><br><br><br>
---

오늘 기억해야 할것

1\. css를 작성할 때는 전체에 적용될 스타일을 먼저 정하고 그 다음 작은거, 좀 더 작은 거 순으로 좁혀 나가야 한다.

[##_Image|kage@bt13uZ/btrBtDoi9Qd/9s8tdQQO16qFsrDxPiWdbk/img.png|CDM|1.3|{"originWidth":308,"originHeight":258,"style":"alignCenter"}_##]

 2. 브라우저의 기본값에 사용자 정의 css가 덮어씌워진다.