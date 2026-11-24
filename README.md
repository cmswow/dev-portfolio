# cmswow 개발 포트폴리오

Windows 키오스크에서 반복되는 설치 작업을 자동화하고, IoT 센서 연결과 전송 상태를 확인하는 도구를 만들었습니다.

## 대표 프로젝트

### R-CMS 설치 자동화

키오스크마다 필요한 프로그램 설치, 서버 시작 설정, 안전보건자료(MSDS) 복사를 하나의 Windows 설치 도구에 묶었습니다.

- **설치 흐름** · C#과 WinForms로 설치 항목과 현재 상태를 표시하고, 무인 진행과 단계별 확인을 지원했습니다.
- **MSDS 증분 복사** · 원본에 있는 PDF 중 대상에 없거나 크기가 다른 파일만 적용합니다. 문서 복사만 따로 실행할 수 있고, 확인·복사·교체 건수를 표시합니다.
- **빌드 재현** · PowerShell로 기존 설치 파일에서 빌드 재료를 복원하고, 변경한 소스로 다시 패키징하는 절차를 구성했습니다.
- **검증 상태** · 0.35 설치 파일은 로컬 빌드를 완료했습니다. 신규 Windows 키오스크 설치 검증은 대기 중입니다.

[설치 도구 소스 · 비공개](https://github.com/cmswow/R-CMS_Setup/tree/release/0.35)

### R-CMS 센서 운영 도구

단독 키오스크와 네트워크 연동 환경에서 IoT 센서 전송을 시작하고, 전송이 끊겼을 때 원인을 확인하는 PowerShell 도구입니다.

- **자동 시작** · Windows 작업 스케줄러를 사용해 로그인 시 환경에 맞는 전송 스크립트를 실행합니다.
- **연결 대기** · 네트워크 연동 모드는 연결을 기다린 다음 전송하고, 실행 중에도 주소 변경을 확인합니다.
- **전송 진단** · 실행 중인 프로세스, 중복 실행, 서버 연결, COM 포트와 전송 로그를 점검합니다.

[센서 도구 소스 · 비공개](https://github.com/cmswow/R-CMS_Sensorset/tree/2026-11-20-v1.0.0)

## 개발 기록

| 작업 | 구현 내용 | 소스 |
| --- | --- | --- |
| Spring 웹 개발 실습 | 회원 등록·조회 예제로 Spring MVC, JDBC와 JPA 저장소, 서비스 테스트 실습 | [inflearn_spring_start](https://github.com/cmswow/inflearn_spring_start) |
| Velog 글 백업 | Python으로 RSS의 새 글을 파일에 저장하고 GitHub Actions 예약 실행을 구성 | [velog](https://github.com/cmswow/velog) |
| 백준 알고리즘 풀이 | Java 제출 코드와 문제 설명 정리 | [BaejoonHub_Algorithm](https://github.com/cmswow/BaejoonHub_Algorithm) |

## 웹 포트폴리오

이 저장소를 내려받아 `index.html`을 브라우저에서 열면 웹 버전을 볼 수 있습니다.

[GitHub 프로필](https://github.com/cmswow)
