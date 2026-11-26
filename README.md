<div align="center">

<a href="https://cbetalk-mcp.netlify.app"><img src="docs/images/banner.png" alt="쪽지 정리는 AI에게, 보내기는 내가. cbetalk-mcp" width="100%"></a>

# cbetalk-mcp

**충북소통메신저(CBE Talk) 쪽지를 AI에게 맡기는 도우미**

안 읽은 쪽지 확인 · 설문 회신 취합 · 받는 사람 찾기 · 쪽지 초안 쓰기를 말 한마디로

<br>

<a href="https://github.com/jkf87/cbetalk-mcp-installer/releases/download/v0.4.0/cbetalk-mcp-setup-0.4.0.exe"><img src="https://img.shields.io/badge/%EC%84%A4%EC%B9%98%20%ED%8C%8C%EC%9D%BC%20%EB%B0%9B%EA%B8%B0-v0.4.0%20%C2%B7%2025MB-1f5fd6?style=for-the-badge&logo=windows&logoColor=white" alt="설치 파일 받기 v0.4.0 · 25MB"></a>
&nbsp;
<a href="https://cbetalk-mcp.netlify.app"><img src="https://img.shields.io/badge/%EC%84%A4%EC%B9%98%C2%B7%EC%82%AC%EC%9A%A9%20%EC%95%88%EB%82%B4-%EA%B7%B8%EB%A6%BC%EC%9C%BC%EB%A1%9C%20%EB%B3%B4%EA%B8%B0-d42a2f?style=for-the-badge" alt="설치·사용 안내 그림으로 보기"></a>

<img src="https://img.shields.io/badge/Windows-10%20%C2%B7%2011-0078D4?style=flat-square" alt="Windows 10 · 11">
<img src="https://img.shields.io/badge/%EA%B4%80%EB%A6%AC%EC%9E%90%20%EA%B6%8C%ED%95%9C-%ED%95%84%EC%9A%94%20%EC%97%86%EC%9D%8C-2ea44f?style=flat-square" alt="관리자 권한 필요 없음">
<img src="https://img.shields.io/badge/Node.js-%ED%8F%AC%ED%95%A8-339933?style=flat-square&logo=nodedotjs&logoColor=white" alt="Node.js 포함">
<img src="https://img.shields.io/badge/Claude%20Code%20%C2%B7%20Codex%20%C2%B7%20Antigravity-%EC%A7%80%EC%9B%90-555?style=flat-square" alt="Claude Code · Codex · Antigravity 지원">

</div>

<br>

## 무엇을 할 수 있나요

| | |
|---|---|
| **쪽지 확인** | "안 읽은 쪽지 보여 줘", "오늘 받은 쪽지 중에 회의 관련만" |
| **설문 취합** | "전학공 음료 주문 설문 취합해 줘" → 수량·금액 합계, 애매한 답, 미회신자를 한 번에 |
| **사람 찾기** | "교무부 이몽룡 선생님 찾아 줘" |
| **쪽지 초안** | "3번 쪽지에 확인했다고 답장 써 줘" → 미리보기를 보고 사람이 보내기 |

쓰는 방법은 두 가지입니다.

- **AI 도구에서**: Claude Code, Codex, Antigravity(agy). 설치할 때 체크만 하면 자동으로 등록됩니다.
- **이 PC 안의 작은 AI(로컬 2B)로**: 쪽지 내용이 외부 AI 서버로 나가지 않습니다. CPU만으로 돌고, 한 번 답하는 데 3~6초 걸립니다.

<br>

## 처음 실행할 때: 파란 경고 창 넘기기

> [!IMPORTANT]
> 코드 서명 인증서를 붙이지 않은 프로그램이라 **"Windows의 PC 보호"** 창이 뜹니다. 바이러스가 발견됐다는 뜻은 아닙니다.
> **추가 정보**는 버튼이 아니라 본문 바로 아래의 **작은 밑줄 글씨**입니다. 여기서 많이 막힙니다.

<table>
  <tr>
    <th width="50%">① 본문 아래 <code>추가 정보</code> 글씨를 누릅니다</th>
    <th width="50%">② 새로 생긴 <code>실행</code>을 누릅니다</th>
  </tr>
  <tr>
    <td><img src="docs/images/ss-1-first.png" alt="Windows의 PC 보호 첫 화면. 추가 정보 글씨에 빨간 동그라미" width="100%"></td>
    <td><img src="docs/images/ss-2-more.png" alt="추가 정보를 누른 뒤 실행 버튼에 빨간 동그라미" width="100%"></td>
  </tr>
  <tr>
    <td><b>실행 안 함</b>을 누르면 설치가 취소됩니다.</td>
    <td>"게시자: 알 수 없는 게시자"는 서명을 안 해서 나오는 문구입니다.</td>
  </tr>
</table>

<details>
<summary><b>'실행' 버튼이 끝까지 안 나온다면</b></summary>
<br>

학교 PC 관리 정책이나 Windows의 '스마트 앱 컨트롤'이 켜져 있으면 실행 버튼 없이 막힙니다.

1. 설치 파일을 **오른쪽 클릭 → 속성**
2. 아래쪽 **보안: 차단 해제**에 체크 → **확인**
3. 다시 실행

그래도 막히면 학교 정보 담당 선생님께 문의하세요.
</details>

<br>

## 설치 순서

<table>
  <tr>
    <td width="33%" valign="top"><b>③ 설치 위치는 그대로 두고 다음</b><br><sub>내 사용자 폴더에 깔려서 관리자 비밀번호를 묻지 않습니다.</sub></td>
    <td width="33%" valign="top"><b>④ 쓸 AI 도구를 체크</b><br><sub>이 PC에 깔린 도구만 보입니다. 로컬 2B 모델(1.4GB)은 선택입니다.</sub></td>
    <td width="33%" valign="top"><b>⑤ 고른 항목을 확인하고 설치</b><br><sub>끝나면 시작 메뉴 <code>cbetalk-mcp → 사용 안내</code>가 생깁니다.</sub></td>
  </tr>
  <tr>
    <td><img src="docs/images/inst-1-dir.png" alt="설치 위치 선택 화면" width="100%"></td>
    <td><img src="docs/images/inst-2-tasks.png" alt="추가 작업 선택 화면" width="100%"></td>
    <td><img src="docs/images/inst-3-ready.png" alt="설치 준비 완료 화면" width="100%"></td>
  </tr>
</table>

<br>

## 이렇게 씁니다

충북소통메신저가 켜져 있고 로그인돼 있어야 합니다. AI 도구는 설치 뒤 한 번 새로 실행하세요.

| 도구 | 준비 | 이렇게 말해 보세요 |
|---|---|---|
| **Claude Code** | `/mcp`에서 `cbetalk`가 보이면 끝 | `안 읽은 쪽지 보여 줘` |
| **Codex** | 도구를 처음 쓸 때 허용 | `3번 쪽지 답장 초안 써 줘` |
| **Antigravity (agy)** | 허용 목록에 `mcp(cbetalk/*)`를 넣으면 매번 묻지 않음 | `지난주 보낸 쪽지에서 연수 일정 찾아 줘` |

### 로컬 2B로 설문 취합

시작 메뉴의 **로컬 모델 받기**(처음 한 번, 1.4GB) → **로컬 모델 대화**. 메신저에 닿지 않는 **연습 모드**도 있습니다.

<p align="center"><img src="docs/images/chat-2.png" alt="로컬 모델이 전학공 음료 주문 설문을 취합한 화면" width="90%"><br><sub>연습 모드에서 설문 회신을 취합한 화면 (이름은 연습용 가명)</sub></p>

<br>

## 믿고 맡길 수 있게

| | |
|---|---|
| **보내기 전에 미리보기** | 보내기·답장·삭제는 기본이 미리보기입니다. 내용을 보고 "보내"라고 해야 실제로 나갑니다. |
| **로컬 AI는 보내지 못함** | 로컬 모델에는 발송 도구가 없습니다. Windows 확인 창에서 사람이 [보내기]를 눌러야 나갑니다. |
| **읽음 표시 조심** | 목록 보기와 설문 취합은 미리보기만 씁니다. 안 읽은 쪽지를 열 때는 한 번 더 묻습니다. |
| **숫자는 프로그램이 계산** | 설문 수량·금액은 AI가 고쳐 쓰지 않고, 계산한 그대로 화면에 나옵니다. |

<br>

## 받은 파일 확인 · 지우기

<details>
<summary><b>받은 파일이 원본 그대로인지 확인하기 (SHA256)</b></summary>
<br>

```powershell
Get-FileHash "$env:USERPROFILE\Downloads\cbetalk-mcp-setup-0.4.0.exe"
```

릴리스의 `SHA256SUMS.txt` 값과 같으면 됩니다.

v0.4.0: `75d44e2c0bb9bd826c105aa5efb32ee7d9d591f638c36a986976cd725b98214e`
</details>

<details>
<summary><b>지우기</b></summary>
<br>

**설정 → 앱 → 설치된 앱**에서 `cbetalk-mcp`를 제거합니다. AI 도구에 등록한 `cbetalk`도 함께 지워집니다. 받은 로컬 모델(`%LOCALAPPDATA%\cbetalk-mcp`)과 쪽지 백업 폴더는 남겨 둡니다.
</details>

<details>
<summary><b>설치 파일에 들어 있는 것</b></summary>
<br>

- cbetalk-mcp 서버와 실행 스크립트
- Node.js 실행 파일 (`node\node.exe`, 라이선스 `node\LICENSE`)
- 로컬 2B 모델은 들어 있지 않습니다. 설치 중에 고르거나 나중에 받습니다 (llama.cpp b10883 + Qwen3.5-2B Q4_K_M).
</details>

<br>

<div align="center">

**제작자: 코난쌤**

<sub><a href="https://cbetalk-mcp.netlify.app">안내 페이지</a> · <a href="https://github.com/jkf87/cbetalk-mcp-installer/releases">모든 버전</a></sub>

</div>
