# 학교 Outlook을 매번 로그인 없이 연결하기

학교 계정(Microsoft 365)은 보통 학교 IT가 외부 앱 연결을 막아 둡니다.
그래서 Claude의 Microsoft 365 커넥터가 "관리자 승인 필요"로 막히는 경우가 많아요.
**학교 비밀번호를 봇에 저장하는 방식은 쓰지 않습니다** (MFA 때문에 동작도 안 하고, 학교 규정 위반 소지).

## 방법 A (추천): Outlook → Gmail 자동 전달

한 번 설정하면 학교 메일이 Gmail로 계속 복사되고, 봇은 Gmail만 보면 됩니다. 로그인 만료 없음.

1. 지금 열어둔 Outlook 웹에서 오른쪽 위 **⚙️ 설정**
2. **메일 → 전달(Forwarding)**
3. **전달 사용(Enable forwarding)** 체크
4. 받을 주소: 내 Gmail 주소
5. **전달된 메시지의 복사본 유지(Keep a copy of forwarded messages)** 체크 ← 꼭!
6. 저장

그 다음 Gmail에서 필터 만들기:
- 검색창 옆 필터 아이콘 → **받는사람(To)**: `@학교도메인` (예: `@school.edu`)
- **필터 만들기** → **라벨 적용: `School`** (+ 원하면 "받은편지함 건너뛰기")

> 전달이 안 되고 `550 5.7.520 Access denied, your organization does not allow external forwarding`
> 같은 반송 메일이 오면 → 학교가 외부 전달을 막은 것. 방법 B/C로.

## 방법 B: Microsoft 365 커넥터 재연결

https://claude.ai/customize/connectors → Microsoft 365 → 재연결.
"관리자 승인 필요" 화면이 뜨면 학교 IT 정책으로 막힌 것.
참고: 이 커넥터는 메일 **검색·읽기 전용**이라, 연결돼도 라벨/답장은 Gmail 쪽에서만 가능.

## 방법 C: 브라우저 세션 이용 (컴퓨터가 켜져 있을 때만)

Claude 데스크톱 앱 + Claude in Chrome 확장을 쓰면, 이미 로그인된 Outlook 탭을 Claude가 직접 읽을 수 있습니다.
단, 컴퓨터가 켜져 있고 브라우저 로그인이 유지될 때만 동작해서 "매일 아침 자동 실행"용으로는 A가 훨씬 안정적입니다.
