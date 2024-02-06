---
aliases:
  - Advanced topics/HTML sanitization
---

Obsidian은 노트를 원하는 대로 표시하거나 [[Embedding web pages|웹 페이지 삽입]]을 할 수 있도록 HTML을 지원합니다. 노트 내에서 HTML을 사용하는 것은 보안 리스크가 따르기 때문에 Obsidian은 노트 내의 모든 HTML을 _검열_ 합니다.

> [!example] 
> `<script>` 요소는 일반적으로 로드될 때마다 JavaScript를 실행할 수 있게 합니다. Obsidian이 HTML을 검열하지 않았다면 공격자가 컴퓨터에서 민감한 정보를 추출하고 그 정보를 다시 공격자에게 보내도록 설계된 JavaScript를 포함한 텍스트를 붙이도록 속일 수 있습니다.

그럼에도 불구하고, 마크다운 구문이 모든 형태의 스타일링을 지원하지 않기 때문에, 검열된 HTML을 사용하면 노트의 품질을 향상시키는 또 다른 방법일 수 있습니다. 일반적인 HTML 사용법 중 일부를 포함하였습니다.

> [!info] `<iframe>` 사용에 대한 자세한 내용은 [[Embedding web pages|웹 페이지 삽입]]에서 확인할 수 있습니다.

### Comments

[[Basic formatting syntax#Comments|마크다운 코멘트]]는 노트 내에서 숨겨진 코멘트를 추가하는 우선적인 방법입니다. 그러나 [Pandoc](https://pandoc.org/)와 같은 마크다운 노트를 변환하는 일부 방법은 마크다운 코멘트를 제한적으로 지원하는 경우가 있습니다. 이러한 경우 `<!-- HTML Comment -->`를 대신 사용할 수 있습니다!

### Underline

노트 내에서 항목을 빠르게 밑줄 표시해야 하는 경우 `<u>예제</u>`를 사용하여 <u>밑줄 표시된 텍스트</u>를 만들 수 있습니다.

### Span/Div

Span 및 div 태그는 [[CSS snippets|CSS 스니펫]]에서 사용자 지정 클래스 또는 사용자 정의 스타일을 선택한 텍스트 영역에 적용하는 데 사용할 수 있습니다. 예를 들어, `<span style="font-family: cursive">당신의 텍스트</span>`를 사용하면 글꼴을 빠르게 <span style="font-family: cursive">바꿀 수 있습니다.</span>

## Strikethrough

<s>텍스트를</s> 취소선 처리해야 하는 경우 `<s>이것</s>`을 사용하여 텍스트를 취소하세요.


