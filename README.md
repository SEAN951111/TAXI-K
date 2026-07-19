# 택시케이 (Taxi-K)

나트랑 한국인 전용 프리미엄 택시 서비스 · 소비자용 하이브리드 앱 **프로토타입**

- 라이브 미리보기(GitHub Pages): 저장소 Settings → Pages 활성화 후 발급되는 링크
- 단일 파일: `index.html` (HTML/CSS/Vanilla JS, 프레임워크 무관 · 인수인계용 주석 포함)

## 주요 기능
- 다국어 UI (한국어 / English / Tiếng Việt)
- 그랩 스타일 장소 선택(자동완성·인기 장소·최근 이용·현재 위치·지도에서 선택) → 정찰제 구역 자동 매핑
- Mock 실시간 GPS 차량 이동 시각화
- 확장형 `PaymentService`(현금·GLN·토스·이니시스·VNPAY·Momo 인터페이스)
- [예약하기] 시 기사앱/Admin 서버로 보낼 JSON 페이로드 출력

## 아키텍처 (Service Layer)
`I18nService · FareService · PlacesService · LocationService · MatchingService · PaymentService · BookingService`
실서비스 전환 지점은 코드 내 `TODO(handoff)` 주석 참조.
