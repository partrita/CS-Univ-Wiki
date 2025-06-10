# SSH (Secure Shell) 및 Telnet

SSH와 Telnet은 원격 컴퓨터에 접속하여 명령을 실행하거나 파일을 전송할 수 있게 해주는 네트워크 프로토콜입니다.

## SSH (Secure Shell)
SSH는 이름에서 알 수 있듯이 보안이 강화된 프로토콜입니다. 클라이언트와 서버 간의 모든 통신을 암호화하여 중간에서 데이터를 가로채더라도 안전하게 보호합니다. 현대적인 원격 접속에서는 SSH 사용이 강력히 권장됩니다.

### 주요 기능
- 원격 터미널 접속
- 파일 전송 (SFTP, SCP 프로토콜 사용)
- 포트 포워딩 (터널링)

### 클라이언트 소프트웨어
- **Windows:**
  - [PuTTY](https://www.putty.org/)
  - Xshell
  - SecureCRT
  - Windows Terminal (내장 OpenSSH 클라이언트 사용 가능)
  - WSL (Windows Subsystem for Linux) 내의 `ssh` 명령어
- **Linux / macOS:**
  - 대부분의 시스템에 기본적으로 `ssh` 명령줄 클라이언트가 내장되어 있습니다. 터미널에서 바로 사용할 수 있습니다.
  ```bash
  ssh username@hostname_or_ip
  ```

## Telnet
Telnet은 SSH보다 먼저 개발된 원격 접속 프로토콜입니다. 하지만 Telnet은 통신 내용을 암호화하지 않아 보안에 매우 취약합니다. 아이디, 비밀번호를 포함한 모든 데이터가 평문으로 전송되므로, 오늘날에는 거의 사용되지 않으며, 사용이 권장되지 않습니다.

특별한 경우(예: 오래된 네트워크 장비 접근, 간단한 포트 체크)를 제외하고는 항상 SSH를 사용하는 것이 좋습니다.

{% include "templates/in-progress.md" %}
