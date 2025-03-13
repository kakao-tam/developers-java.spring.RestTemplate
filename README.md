# Spring Boot 카카오 API 연동 프로젝트

이 프로젝트는 Spring Boot를 사용하여 카카오 API를 연동하는 예제 프로젝트입니다.

## 기술 스택

- Java 21
- Spring Boot 3.2.3
- Gradle 8.x
- Lombok
- Spring Validation

## 시작하기

1. 프로젝트 클론
2. 애플리케이션 실행:
   ```bash
   ./gradlew bootRun
   ```
3. 브라우저에서 http://localhost:8080 접속

## 카카오 API 설정

1. [카카오 개발자 콘솔](https://developers.kakao.com)에서 애플리케이션 생성
2. 카카오 로그인 활성화
3. Redirect URI 설정: http://localhost:8080/api/kakao/redirect
4. JavaScript 키와 REST API 키를 `application.yml`에 설정

## 주요 기능

- 카카오 로그인
- 사용자 프로필 조회
- 친구 목록 조회
- 카카오톡 메시지 전송
- 로그아웃
- 연결 끊기

## API 엔드포인트

- `/api/kakao/authorize`: 카카오 로그인 인증
- `/api/kakao/redirect`: 카카오 로그인 콜백
- `/api/kakao/profile`: 사용자 프로필 조회
- `/api/kakao/friends`: 친구 목록 조회
- `/api/kakao/message`: 카카오톡 메시지 전송
- `/api/kakao/logout`: 로그아웃
- `/api/kakao/unlink`: 연결 끊기

## 에러 처리

- API 호출 시 발생하는 에러 메시지를 클라이언트에 전달
- HTTP 상태 코드별 에러 응답 처리
- 세션 기반의 토큰 관리

## 스크린샷
<img width="816" alt="image" src="https://github.com/user-attachments/assets/e31e71d8-f8c4-4759-94f3-439834741433" />

