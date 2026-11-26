# cbetalk-mcp 설치 파일

충북소통메신저(CBE Talk) 쪽지를 AI 도구(Claude Code, Codex, Antigravity)나 이 PC 안의 작은 AI(로컬 2B)로 다루게 해 주는 **cbetalk-mcp**의 Windows 설치 파일을 배포하는 곳입니다.

- 안 읽은 쪽지 확인, 설문 회신 취합, 받는 사람 찾기, 쪽지 초안 쓰기를 말로 시킬 수 있습니다.
- 쪽지는 사람이 확인해야 나갑니다. 보내기는 미리보기부터 보여 줍니다.

## 받기

[**Releases**](https://github.com/jkf87/cbetalk-mcp-installer/releases)에서 `cbetalk-mcp-setup-<버전>.exe`를 받습니다.

- Windows 10·11, 관리자 권한 필요 없음, Node.js를 따로 설치하지 않아도 됩니다.
- 받은 파일이 원본인지 확인하려면 PowerShell에서 `Get-FileHash <파일>`을 실행해 릴리스의 `SHA256SUMS.txt` 값과 비교합니다.

## 처음 실행할 때 파란 경고 창이 뜹니다

코드 서명 인증서를 붙이지 않은 프로그램이라 "Windows의 PC 보호" 창이 뜹니다.

1. 본문 바로 아래의 작은 밑줄 글씨 **추가 정보**를 누릅니다. (**실행 안 함**을 누르면 설치가 취소됩니다)
2. 새로 생긴 **실행** 버튼을 누릅니다.

그림과 함께 보는 설치·사용 안내는 안내 페이지에 있습니다.

## 포함된 것

- cbetalk-mcp 서버와 실행 스크립트
- Node.js 실행 파일(`node\node.exe`, Node.js 라이선스는 `node\LICENSE`)
- 로컬 2B 모델은 들어 있지 않습니다. 설치 중에 고르거나 나중에 시작 메뉴 "cbetalk 로컬 모델 받기"로 받습니다(llama.cpp b10883, Qwen3.5-2B Q4_K_M, 약 1.4GB).

제작자: 코난쌤
