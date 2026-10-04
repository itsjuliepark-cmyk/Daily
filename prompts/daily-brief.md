# 매일 아침 브리핑 (Routine 프롬프트)

CLAUDE.md와 rules.md를 읽고 그대로 따른다.

1. Gmail에서 최근 24시간 메일을 가져온다 (spark@mba2028.hbs.edu 학교 메일도 Gmail로 들어옴).
   Microsoft 365 커넥터가 연결돼 있으면 Outlook도 직접 검색해서 빠진 게 없는지 확인한다.
2. rules.md 기준으로 🔴/🟠/🟢/⚪ 분류.
3. 🔴 커피챗/일정 조율: Google Calendar에서 빈 시간을 찾아 답장 **초안**을 만들고 data/coffee-chats.md 갱신.
4. 🟠 마감: 날짜순 정리, 캘린더에 없는 마감은 목록에 표시 (자동 등록은 하지 않음).
5. ⚪ 노이즈: Gmail 라벨 `Daily/⚪노이즈` 부착 (다른 분류도 각 Daily/ 라벨 부착).
6. CLAUDE.md의 출력 형식으로 카카오톡 "나에게 보내기"로 요약 전송.
7. data/ 변경사항은 커밋 후 푸시.
