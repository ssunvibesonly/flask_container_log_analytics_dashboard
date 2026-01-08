<<<<<<< HEAD
# flask_container_log_analytics_dashboard
Flask 활용한 학습용 프로젝트
=======
# 로그 분석 대시보드 백엔드

이 프로젝트는 컨테이너 로그 데이터를 분석하고 시각화하기 위한 Flask 기반 백엔드입니다. 프론트엔드 애플리케이션(예: Chart.js)에서 사용할 수 있도록 집계된 로그 통계를 제공하는 API를 제공합니다.

이 프로젝트는 일관된 구조를 보장하기 위해 AI 협업 가이드라인(gemini.md)과 Cursor 규칙을 포함하고 있습니다.

## 주요 기능

- **로그 파이프라인**: Docker 컨테이너를 이용한 `producer` -> `collector` -> `database` 파이프라인.
- **RESTful API**: 통계 데이터(타임라인, Top-N 등)를 제공하는 Flask API.
- **확장 가능한 구조**: Flask의 앱 팩토리(App Factory)와 블루프린트(Blueprint) 패턴으로 설계.
- **단일 명령어로 전체 시스템 실행**: 모든 서비스는 Docker Compose를 통해 관리.

## 사전 준비물

- Docker
- Docker Compose

## 시작하기

1.  저장소를 복제합니다:
    ```bash
    git clone <your-repo-url>
    cd flask_container_log_analytics_dashboard
    ```

2.  서비스를 빌드하고 실행합니다:
    ```bash
    docker-compose up --build
    ```

3.  API는 `http://localhost:5001` 주소에서 실행됩니다.
    -   API 상태 확인: `curl http://localhost:5001/ping`
>>>>>>> c34f101 (repo 생성 전 원격에 먼저 올라간 이슈 해결)
