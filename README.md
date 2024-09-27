# ✈️ 누구나 접근할 수 있는 항공사 웹사이트

## 목표

- 항공사 웹사이트 컴포넌트의 스크린 리더 접근성 높이기
  - 이미지 캐로셀 컴포넌트의 접근성 개선
  - 항공사 웹사이트의 모바일 페이지 1개의 접근성 개선 목표

## 학습 목표 : 최소한의 마크업으로 최대한의 접근성 확보하기

- 시맨틱 태그를 사용해 웹 페이지의 구조를 명확히 하고, 의미를 직관적으로 전달.
- 최소한의 마크업을 사용해 불필요한 요소를 줄이고, HTML의 기본 기능 최대한 활용.
- ARIA 속성은 꼭 필요한 경우에만 사용하여 추가적인 정보 제공.
  - No ARIA is better than Bad ARIA
- 시각적 표현과 접근성을 모두 만족시키는 방법 함께 고민.

## 기능 요구 사항

### 1) 컴포넌트 접근성 개선 - 이미지 캐로셀

- [ ] 스크린 리더가 캐로셀의 전체 아이템 수를 읽을 수 있다.
- [ ] 스크린 리더가 이미지 캐로셀 내 각 아이템 정보를 읽을 수 있다.
- [ ] 여행지, 좌석 유형, 가격 정보를 한번에 읽을 수 있다.
- [ ] 이전/다음 아이템으로 이동하고 현재 보이는 아이템의 정보를 읽을 수 있다.
- [ ] 각 아이템을 선택하면 각각에 맞는 링크로 이동할 수 있다.

### 2) 페이지 접근성 개선

- [ ] 페이지를 하나의 문서로 읽을 수 있다.
- [ ] 페이지에 적절한 제목(title) 제공. 제목은 페이지의 주요 내용을 간결하게 설명한다.
- [ ] 페이지의 주요 영역을 시맨틱 태그를 사용해 명확히 구분한다.
- [ ] heading을 논리적인 순서로 사용해 페이지 구조를 명확히 한다.
- [ ] 키보드 사용자를 위해 페이지 최상단에 '본문으로 바로가기' 링크를 제공해 반복되는 메뉴를 건너뛸 수 있게 한다.
  - (a.k.a. skip link / skip navigation. cf. github.com)

### 선택 요구 사항 - 팝업 모달 포커스 트랩

- [ ] 스크린 리더로 진입했을 때에도 현재 팝업이 떴다는 것을 인지할 수 있다.
- [ ] 팝업이 열려있는 동안에는 포커스 이동이 팝업 내에서만 이루어진다.
- [ ] 스크린 리더로 팝업을 닫을 수 있다.
- [ ] 키보드 접근성을 함께 고려한다.
  - [ ] 키보드만으로도 팝업으로 바로 진입해서 팝업을 닫을 수 있다

## 접근성 체크리스트

- 접근성 문제 정의 및 우리 서비스에서 챙길 접근성 체크리스트 v1 만들기
- 우리 팀에서 가장 중요하고 자주 사용되는 기능 플로우 : 방 만들기 -> 닉네임 입력 -> 다른 사용자 초대 -> 게임 시작 -> 밸런스 게임 옵션 선택 -> 라운드 결과 확인
- [ ] 화면을 볼 수 없는 사용자가 이 단계를 완료할 수 있는가?
- [ ] 이 단계에서 제공하는 정보나 지시 사항이 모든 사용자에게 명확한가?
- 팀원들과 함께 각 질문을 바탕으로 의견을 나누고, 우리 팀 서비스에서 우선순위 높게 챙길 접근성 체크리스트 만들기
  - ex. "모든 이미지와 인터랙티브 요소에 적절한 대체 텍스트가 제공되는가?"
