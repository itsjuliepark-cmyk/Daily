# 링크드인 아웃리치 규칙 (자유롭게 고치세요)

"○○ 회사 △△ 직무 사람 찾아줘" → 사람을 찾고 메시지 초안을 만든다.
"보내줘" → 사용자가 고른 사람에게만 보낸다. 기록은 `data/linkedin-outreach.md`.

## 내 소개 (메시지 첫 문장 — 바뀌면 여기만 고치기)
- 이름: Julie
- 지금: HBS RC (1학년, MBA 2028)
- 이전: SK Telecom 마케팅 + AI 프로덕트
- 지금 노리는 것: 요청에 회사/직무가 없으면 물어본다 (예: Adobe MBA PM 인턴십)

## 메시지 형식 (링크드인 연결 메모 — **200자 이하**)
링크드인 Add a note 칸이 200자까지만 들어간다 (10/8 확인 — 300자 버전은 너무 길었음).
```
Hi [이름], I’m Julie, an HBS RC, ex-SK Telecom marketing & AI product.
[개인화 한 문장 — 약 50–60자]
I’m pursuing [회사]’s MBA [직무] internship. Could we chat for 15 min?
```
예시 (198자):
> Hi Mehreen, I’m Julie, an HBS RC, ex-SK Telecom marketing & AI product. Your path from Adobe’s PM internship to full-time resonates. I’m pursuing Adobe’s MBA PM internship. Could we chat for 15 min?

- 고정 부분이 약 130자 + 이름 → **개인화 문장은 60자 안쪽**, 전체 **200자 이하** (글자 수 세서 같이 표시).
- 수락 후 첫 메시지(1촌 Message)는 길이 제한이 없으니, 거기서 "I’d truly value your advice" 같은 말과 구체적인 질문을 덧붙인다.
- 상대가 HBS 같은 학년이면 "a fellow HBS RC"로 쓴다.
- 같은 회사 사람끼리 메시지를 비교할 수 있으니 개인화 문장의 동사를 조금씩 다르게 (resonates / inspires me 등).

## 개인화 문장 규칙
- 프로필에 **실제로 있는 사실** 1–2개만 쓴다: 경력 전환(예: 마케팅 → PM), 담당 제품, MBA 인턴 → 풀타임 전환, HBS 동문, 한국/SKT 연결.
- 내 배경(마케팅, AI 프로덕트)과 이어지는 점을 고른다.
- 확실하지 않은 건 쓰지 않는다 (재학/졸업, 정확한 팀명 등 — 애매하면 "Your path from HBS to product at Adobe"처럼 넓게).
- 과한 칭찬, 개인 게시물·사생활 언급 X.

## 사람 찾는 기준 (우선순위 순)
- **기본: 지금 그 회사에서 풀타임으로 일하는 사람만** (재학생·인턴만 한 사람은 제외 — 10/6 사용자 요청). 프로필의 현재 직책·시작 날짜로 확인.
- **근무 국가도 확인**: 미국 인턴십이면 지금 미국에서 일하는 사람만. 검색 결과만 믿지 말고 프로필을 열어 현재 직책의 도시를 확인한다 (해외 이동한 경우가 있음).
1. 목표 회사에서 일하는 **HBS 동문**, 특히 MBA 인턴 → 풀타임 전환한 사람
2. 내 배경과 비슷한 사람: 마케팅 → PM 전환, AI 프로덕트, 한국 회사 출신(삼성·SKT 등)
3. 다른 MBA 출신으로 MBA 인턴 → 풀타임 전환한 사람
4. 다른 MBA 출신으로 목표 직무에 있는 사람
- 제외: `data/linkedin-outreach.md`(제외/보류 포함)나 `data/coffee-chats.md`에 이미 있는 사람, 이미 회사를 떠난 사람, VP 이상 임원(요청 시만)
- 한 번에 5명 안팎. 검색 결과가 오래됐을 수 있으니 현재 직책이 확실하지 않으면 표시한다.

## 찾는 방법
- Exa 검색 `category:people` (링크드인 프로필이 나옴) — 예: `category:people Harvard Business School MBA product manager at Adobe`
- 필요하면 회사·직무·키워드를 바꿔 2–3번 검색해서 합친다.

## 결과 보여주는 형식 (채팅)
```
1. 이름 — 직책 @ 회사 · 학교
   🔗 linkedin.com/in/...
   왜: (한 줄 — 왜 이 사람인지)
   ✉️ (메시지 전문) — 281자
```
→ `data/linkedin-outreach.md`에 상태 "초안"으로 추가.

## "보내줘" 처리
- 사용자가 **이름을 콕 집은 사람에게만** 보낸다. "다 보내줘"면 그 목록 전체.
- 사용자가 본 문구 그대로 보낸다. 고쳤으면 고친 최종본을 다시 보여준다.
- **Claude in Chrome / 컴퓨터 사용이 연결된 경우** (데스크톱 앱): 사용자의 로그인된 링크드인에서 프로필 열기 → Connect → Add a note → 메시지 붙여넣기 → Send. 한 명씩, 끝나면 결과 보고.
  - 이미 연결된 1촌이면 Connect 대신 Message로 보낸다.
  - 하루 10–15명 이하로 (계정 제한 방지).
- **연결 안 된 경우** (클라우드 세션 등 링크드인에 접근 불가): 직접 누를 수 없으니 복사하기 쉽게 사람별 최종본 + 링크를 정리해서 준다. 그래도 상태는 "보냄 대기"로 기록.
- 보낸 뒤 `data/linkedin-outreach.md` 상태를 "보냄 (날짜)"로 바꾸고 커밋·푸시.

## 이후 추적 (매일 브리핑과 연결)
- 수락·답장 알림 메일(@linkedin.com)이 `data/linkedin-outreach.md`에 있는 사람이면 🔴로 분류하고 상태 갱신.
- 커피챗 일정이 잡히면 `data/coffee-chats.md`로 옮긴다.
- 보낸 지 1주 넘게 응답 없으면 브리핑에 한 줄로 알려준다 (후속 메시지 초안 제안).
