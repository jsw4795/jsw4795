# 정성욱

Java / Spring 기반 백엔드 개발자를 목표로 하고 있습니다.

현재 Spring Boot 기반 교통 알림 서비스 [StopBell](https://github.com/jsw4795/stopbell)을 개발하고 있습니다. Google 로그인·토큰 인증과 버스 노선·정류장 저장·갱신을 구현했으며, 교통 API 연동과 알림 기능은 구현 전입니다.

## 대표 프로젝트

### [Cabbage Market](https://github.com/jsw4795/Cabbage_Market) — 중고거래 서비스

**6인 팀 프로젝트 · 담당: 채팅 기능, 팀원 코드 통합**

`Java` `Spring MVC` `MyBatis` `Oracle` `SSE`

- **채팅 구현** — 게시글별 판매자·구매자 채팅방과 메시지·사진 전송을 구현했습니다. 메시지 전송은 HTTP/AJAX, 서버→클라이언트 이벤트 전달은 SSE로 구성했습니다.
- **연결 관리** — 사용자별 `SseEmitter`를 관리하고, 연결 종료·타임아웃·전송 실패 시 emitter를 제거하도록 구현했습니다.
- **재연결 처리** — 이벤트 ID와 최근 이벤트 캐시를 두고, `Last-Event-ID` 이후 이벤트 중 캐시에 남은 항목을 재전송하도록 구현했습니다.
- **업로드 문제 해결** — 프로젝트 내부 리소스에 저장한 사진이 늦게 반영되던 문제를, 저장 경로를 프로젝트 외부로 분리해 개선했습니다.

[채팅 시연과 구현 상세 보기 →](https://github.com/jsw4795/Cabbage_Market#채팅-기능)

## 다른 프로젝트

- **[Wine Manager](https://github.com/jsw4795/wine-manager)** — Spring Boot 기반 개인 와인 구매·소비 기록 서비스. 사용자별 타임라인과 재고 통계를 구현했습니다.
- **[Music Station](https://github.com/jsw4795/Music_Station)** — 4인 팀 음악 공유 서비스. TOP100 조회 결과를 5분 주기로 메모리에 갱신해 응답에 재사용하도록 구현했습니다.
