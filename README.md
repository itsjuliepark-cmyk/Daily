# Daily — 메일 관리 봇

학교 Outlook + 개인 Gmail(커피챗) 메일을 매일 아침 자동으로 분류하고,
답해야 할 것 / 마감 / 이벤트 / 노이즈로 정리해서 카카오톡으로 요약을 보내주는 봇.

## 구조

| 파일 | 역할 |
|---|---|
| `CLAUDE.md` | 봇의 동작 규칙 (분류 기준, 안전 규칙, 출력 형식) |
| `rules.md` | 내가 직접 고치는 분류 규칙 (중요 발신자, 키워드, 무시할 것) |
| `data/coffee-chats.md` | 커피챗 기록 — 누구와, 언제, 후속 조치 |
| `prompts/daily-brief.md` | 매일 아침 자동 실행(Routine)에 쓰는 프롬프트 |
| `docs/outlook-setup.md` | 학교 Outlook을 로그인 없이 연결하는 방법 |

## 셋업 순서

1. **Gmail / Google Calendar 연결** — https://claude.ai/customize/connectors
2. **학교 Outlook → Gmail 자동 전달 설정** — `docs/outlook-setup.md` 참고 (한 번만 하면 끝)
3. **Gmail 필터** — 전달된 학교 메일에 `School` 라벨 자동 부착
4. 새 세션에서 "매일 아침 브리핑 Routine 만들어줘" → 매일 자동 실행
