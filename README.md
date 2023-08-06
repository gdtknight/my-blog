# 원티드 프리온보딩 백엔드 인턴십 - 선발 과제 제출용 리포

- 지원자 : 신용호

## Application 실행 방법

### PreRequisites
- JDK 버전 : 17 이상
- Docker
- IntelliJ
  - `EnvFile` 플러그인 설치 권장
  - 실행 환경에서 아래와 같이 설정

### Docker Compose 실행

- 프로젝트 루트에 `.env` 파일 생성 후 아래의 내용 기입
- ```
    BASIC_BOARD_USER={DB 사용자 ID}
    BASIC_BOARD_PASSWORD={DB 사용자 패스워드}
    BASIC_BOARD_DATABASE=myboard
    BASIC_BOARD_PORTS=3388:3306
    BASIC_BOARD_DB_URL=jdbc:mysql://127.0.0.1:3388/myboard
  ```

- 터미널에서 프로젝트 루트 디렉토리로 이동하여 아래 명령어 실행
  - Windows
   ```
    docker-compose up -d
   ```
  - MacOS, Linux, Git-Bash 등
   ```
    docker compose up -d
   ```
  
### gradle 빌드 및 실행

- 상기 방법을 적용하지 않을 경우 `jar` 파일 실행시 아래와 같이 옵션 부여
  ```
  java -jar basic-board-0.0.1-SNAPSHOT.jar \
  --server.port=8892 \
  --spring.datasource.url='jdbc:mysql:127.0.0.1:3388/myboard' \
  --spring.datasource.username='' \
  --spring.datasource.password=''
  ```
  
### 엔드포인트 호출 방법

- POSTMAN, TALEND API TESTER 등을 이용
- http://localhost:8080/ 으로 HTTP 요청 

## 데이터베이스 테이블 구조

- 

## API 명세 (Request / Response 포함)

- 
구현한 API의 동작을 촬영한 데모 영상 링크
구현 방법 및 이유에 대한 간략한 설명
API 명세(request/response 포함)
