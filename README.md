# 터치 터치 ATM

## 📋 프로젝트 소개

**터치 패널을 탑재한 아이들용 ATM 교육 시스템으로 실제 ATM과 유사한 기능을 갖춘 금융 교육 시뮬레이터**

- **프로젝트 기간**: 2025.01 ~ 2025.02
- **개발 환경**: C, Linux, MariaDB, 프레임버퍼, ARM 아키텍처

---

## 💡 프로젝트 개요

아이들이 금융 거래에 대해 배울 수 있도록 실제와 유사한 ATM 인터페이스를 제공하는 교육용 시스템입니다.
라즈베리파이 기반으로 제작되었으며, 사용자 인증부터 입금, 출금, 송금까지 실제 ATM의 주요 기능들을 모두 구현했습니다.

시스템은 직관적인 터치스크린 인터페이스를 통해 사용자 경험을 제공하며, 보안을 위한 CCTV 기능까지 갖추고 있습니다.
모든 거래 내역은 데이터베이스에 기록되어 금융 교육의 효과를 높입니다.

---

## 📺 Demo

### 📷 시스템 이미지

<table>
  <tr>
    <td align="center" width="50%">
      <img src="https://github.com/user-attachments/assets/e8a9cf18-d4ed-4474-829c-38947651a833" width="450px">
      <br>
      <b>ATM 로그인 화면</b>
    </td>
    <td align="center" width="50%">
      <img src="https://github.com/user-attachments/assets/89a18f45-d4b7-4f78-ae20-9f6aebbbd9df" width="450px">
      <br>
      <b>ATM 메인 화면</b>
    </td>
  </tr>
  <tr>
    <td align="center" width="50%">
      <img src="https://github.com/user-attachments/assets/9f22b7e9-16fa-4a35-91a4-8e69e97f78dd" width="450px">
      <br>
      <b>ATM 거래 화면</b>
    </td>
    <td align="center" width="50%">
      <img src="https://github.com/user-attachments/assets/0a70a7d5-c7ca-4493-b8dc-557d46a1feae" width="450px">
      <br>
      <b>ATM 거래 완료 화면</b>
    </td>
  </tr>
</table>

### 🎬 시연 영상

<div align="left">
  <a href="https://www.youtube.com/playlist?list=PLRV3YgAS3RKiws1OOEKEHuDXr9qPnzZbp" target="_blank">
    <img src="https://img.shields.io/badge/YouTube-OHSY%20ATM%20시연%20영상-red?style=for-the-badge&logo=youtube" alt="시연 영상">
  </a>
</div>

---

## 👥 팀원 소개

<div align="center">

| **오경택(팀장)** | **홍훈의(부팀장)** | **송가람(조원)** | **유승경(조원)** |
| :------: | :------: | :------: | :------: |
| [<img src="https://github.com/user-attachments/assets/4e865b7d-c93f-477d-af75-31c7ac30d4ce" height=150> <br/> gyeongtaek.dev@gmail.com](#) | [<img src="https://github.com/user-attachments/assets/c18a97f8-7f4b-417e-96ff-4cec6845e58b" height=150> <br/> asdfzxcv5621@naver.com](#) | [<img src="https://github.com/user-attachments/assets/c3fa63e1-9026-4acb-8346-1061da44427c" height=150> <br/> sjjsy9634@naver.com](#) | [<img src="https://github.com/user-attachments/assets/5c0fcae8-b865-4f9f-9c60-88eed3e1058c" height=150> <br/> tmdrud7766@gmail.com](#) |

</div>
<br>

---

## ⚙️ 프로젝트 구성

### 🔧 하드웨어
- **메인 보드**: 라즈베리파이 (ARM 아키텍처)
- **디스플레이**: 터치스크린 (800x480)
- **카메라 모듈**: CCTV 기능 제공
- **입력 장치**: 터치스크린 이벤트 처리
- **저장 장치**: SD 카드 및 외부 저장소

### 💻 소프트웨어
- **운영체제**: 리눅스 기반
- **데이터베이스**: MariaDB
- **그래픽 인터페이스**: 프레임버퍼 기반 자체 UI 라이브러리
- **미디어 처리**: ffmpeg (영상 압축 및 저장)

### 🌐 네트워크
- 클라이언트-서버 구조
- TCP/IP 소켓 통신
- CCTV 영상 전송 기능

### 📊 코드 구성도

![스크린샷 2025-05-05 165107](https://github.com/user-attachments/assets/610487d7-ae6b-4aac-8625-5e758643de14)

---

## 🛠️ 주요 기능

### 🔒 사용자 인증
- ID/PW 기반 로그인 시스템
- 잘못된 정보 입력 시 경고 메시지
- 보안을 위한 비밀번호 마스킹 처리

### 💰 금융 거래
- **계좌 조회**: 실시간 잔액 확인
- **입금**: 계좌에 금액 입금 및 잔액 업데이트
- **출금**: 계좌에서 금액 인출 (잔액 초과 시 경고)
- **송금**: 다른 계좌로 금액 이체 (트랜잭션 처리)

### 🖥️ 인터페이스
- 직관적인 터치 기반 UI
- 둥근 모서리 버튼 및 사용자 친화적 디자인
- 커서 깜빡임 효과로 입력 위치 표시
- 숫자 키패드 구현

### 📹 보안 기능
- CCTV 실시간 모니터링
- 60초 단위 영상 저장 및 압축
- 저장된 영상 원격 서버 전송

### 🔄 멀티스레딩
- 터치 이벤트 처리 스레드
- UI 렌더링 스레드
- 영상 처리 및 전송 스레드

---

## 🔑 맡은 역할

- 프레임버퍼 기반 UI 라이브러리 개발
- 터치스크린 이벤트 처리 시스템 구현
- CCTV 영상 저장 및 전송 시스템 개발

---

## ⚠️ 문제와 문제해결

### 1️⃣ 터치스크린 좌표 맵핑 문제

- **문제점**: 터치스크린의 raw 입력값과 디스플레이 좌표 간 불일치
- **해결책**: `scale_value()` 함수를 구현하여 터치스크린 입력값을 디스플레이 좌표로 변환
- **향후 개선점**: 자동 캘리브레이션 기능 구현

### 2️⃣ 멀티스레드 동기화 이슈

- **문제점**: 여러 스레드가 동시에 화면에 그리기 작업 수행 시 깜빡임 현상 발생
- **해결책**: 각 스레드의 역할을 명확히 분리하여 UI 스레드와 이벤트 처리 스레드로 구분

### 3️⃣ 데이터베이스 트랜잭션 관리

- **문제점**: 송금 중 오류 발생 시 데이터 일관성 유지 어려움
- **해결책**: 트랜잭션 기반 쿼리 처리 구현 (START TRANSACTION, COMMIT, ROLLBACK)

---

## 🔮 향후 발전 방향

- 지폐 인식 기능 구현현
- 웹 인터페이스 연동
- 사용자 행동 분석 및 보안 강화
- 기능과 다양성을 늘려 다양한 분야의 교육 시스템에서의 활용용

---

## 🏁 결론

터치 터치 ATM은 아이들에게 금융 교육을 제공하는 효과적인 도구로 개발되었습니다. 실제 ATM과 유사한 기능을 통해 금융 거래의 기본 개념을 체험할 수 있으며, 사용자 친화적인 인터페이스와 보안 기능을 갖추었습니다.

프로젝트 개발 과정에서 프레임버퍼 기반 그래픽 처리, 멀티스레딩, 데이터베이스 연동 등 다양한 기술적 도전을 극복하였으며, 이를 통해 임베디드 시스템 개발 역량을 크게 향상시켰습니다.

향후 더 많은 기능과 개선을 통해 더욱 완성도 높은 교육용 ATM 시스템으로 발전시킬 계획입니다.
