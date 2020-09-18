개념
- 서버를 추상적으로 제공
   - 개발자가 운영과 관련된 문제를 걱정하지 않고 코드 개발에만 집중할 수 있다
- 기능이 필요한 횟수와 시간에 따라 비용을 청구
- AWS에서는 람다 서비스로 제공

람다 계층
- 사용자 지정 런타임을 업로드해서 사용 가능하다

특징
- 완전 관리형 서비스
- 다른 AWS 서비스들을 호출해서 자신만의 서비스를 만들 수 있다
- 요청이 올 때만 프로비저닝 되기 때문에 응답이 없을 때 비용이 청구되지 않는다
   - 이벤트에 대한 응답으로 실행된다

아키텍쳐
1. 입력 인자: 이벤트소스(트리거)
   - HTTP 요청
   - 서버 이상 감지
   - 파일 업로드
   - 데이터 삽입 등
2. 함수: 람다 함수
3. 출력 인자: API로 접근 가능한 모든 서비스
   - 외부 API
   - AWS 서비스
   - 콘솔 출력
   