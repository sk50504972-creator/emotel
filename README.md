# 이모텔 고객 앱 (v2, 2026-10-27)

손님 휴대폰에 설치하는 안내 PWA. 서버 없음. 라이브: https://balhae.claimworks.kr/emotel/

- AI 상담(기기 내 자동응답): 요금·시간·주차·위치·예약·연장 등 FAQ, 어려운 질문은 전화/문자로 연결
- 혜택: QR(`?ref=qr`)로 열면 「앱 설치 환영 쿠폰」 자동 발급, 스탬프 카드, 친구 공유(`?ref=share`). 쿠폰 사용·스탬프 적립은 관리자 앱(이모텔 매니저 › 마케팅 › 앱 혜택·QR)의 **일일 승인번호**로 직원이 확인
- `?ref=room&r=301` 형식 QR은 내 객실 번호를 자동 입력 (객실 테이블텐트용, 관리자 앱에서 A4 인쇄)
- 업소 정보·요금·혜택 문구는 index.html 안 `INFO` 블록만 수정. 승인번호 비밀값 `INFO.benefit.secret`은 관리자 앱 설정과 같아야 함. 고친 뒤 sw.js CACHE_VERSION을 올린다.
- 관리자 앱(별도): https://balhae.claimworks.kr/emotel-crm/
