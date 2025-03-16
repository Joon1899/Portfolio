# RecnRoll 

## Description 
RecnRoll은 실시간 치지직 스트리밍 녹화 프로그램입니다. 사용자가 관심 있는 스트리머를 설정하면, 자동으로 방송 시작을 감지하고 녹화합니다.
설정을 통해 녹화 시작 및 종료 시간 조정, 방송 시작 알림, 다운로드 시작 알림을 개별적으로 설정할 수 있으며, 녹화된 방송은 지정된 폴더에 자동 저장됩니다.
저장된 영상은 RecnRoll 내 기본 동영상 재생 프로그램을 통해 바로 확인할 수 있으며, 알림 설정 및 기록은 Firestore DB에 저장되어 별도의 알림 페이지에서 확인할 수 있습니다.


## 주요 기능 
실시간 스트리밍 감지 및 자동 녹화
녹화된 방송을 지정 폴더에 자동 저장
방송 시작 및 다운로드 알림 기능 (Firestore 연동)
내장 동영상 플레이어를 통한 영상 재생 지원
Firebase 인증 기반 사용자 로그인
## Target OS 
Mac(x64), Window

## 기술 스택 

### GUI 프레임워크
Electron 
Mac 및 Windows 환경에서 실행 가능한 데스크톱 애플리케이션 GUI 구현

### 프론트 엔드
React 
사용자 인터페이스 구현 


### 백 엔드 
Node.js 
사용자 인증 서버: Firebase 기반 사용자 검증 및 토큰 재발급
프록시 서버: Electron Main Process에서 동작하는 프록시 서버를 통해 치지직 API 데이터를 Renderer Process로 전달

### 사용자 인증
Google Firebase Authentication
Google 계정 로그인 지원 (팝업을 통한 OAuth 2.0 인증 방식)

### 데이터베이스(DB)
Google Firestore 
알림 기록 저장 

## 시연 영상 



