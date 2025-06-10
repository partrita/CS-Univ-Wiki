# 디버거 (Debugger)

디버거는 소프트웨어 개발 과정에서 프로그램의 오류(버그)를 찾아내고 수정하는 데 사용되는 필수적인 도구입니다. 프로그램의 실행을 단계별로 제어하고, 변수의 값을 확인하며, 메모리 상태를 분석하는 등의 기능을 제공하여 문제의 원인을 파악하는 데 도움을 줍니다.

## 디버거의 종류 및 소개

다양한 프로그래밍 언어와 환경에 따라 여러 종류의 디버거가 존재합니다. 주요 디버거들은 다음과 같습니다.

### Visual Studio Debugger
Microsoft Visual Studio 통합 개발 환경(IDE)에 내장된 디버거입니다. C++, C#, VB.NET 등 .NET 환경 및 Windows 기반 애플리케이션 개발 시 강력한 디버깅 기능을 제공합니다. 사용자 친화적인 GUI와 다양한 분석 도구를 갖추고 있습니다.

### GDB (GNU Debugger)
GNU 프로젝트의 일부로 개발된 커맨드 라인 인터페이스(CLI) 기반의 디버거입니다. 주로 C, C++ 등 네이티브 언어로 작성된 프로그램을 디버깅하는 데 사용되며, Linux 및 macOS 환경에서 표준 디버거로 널리 사용됩니다.
- **특징**: 강력한 기능과 유연성을 제공하지만, CLI 환경이 익숙하지 않은 사용자에게는 다소 어려울 수 있습니다. 다양한 프론트엔드(GUI) 도구나 확장 기능을 통해 사용성을 개선할 수 있습니다. (예: `gdb-dashboard`)
- **자료**:
  - [GDB 공식 문서](https://www.gnu.org/software/gdb/documentation/)
  - [GDB를 이용한 디버깅 (5판 한국어 번역, 1998년 작성)](http://korea.gnu.org/manual/release/gdb/gdb.html)
  - [gdb 사용법 치트시트](http://www.viper.pe.kr/docs/gdb-manual.html)
  - [gdb-dashboard](https://github.com/cyrus-and/gdb-dashboard) (개선된 GDB 인터페이스)

### LLDB
LLVM 프로젝트의 디버거로, GDB의 대안으로 개발되었습니다. Clang 컴파일러와 함께 사용되며, 특히 macOS 환경에서는 기본 디버거로 사용됩니다. GDB와 유사한 명령어 체계를 가지면서도 표현력 있는 출력과 스크립팅 기능 등 개선된 점들이 있습니다.
- **자료**:
  - [The LLDB Debugger (공식 사이트)](http://lldb.llvm.org/)
  - [Xcode LLDB 디버깅 테크닉](http://www.letmecompile.com/xcode-lldb-%EB%94%94%EB%B2%84%EA%B9%85-%ED%85%8C%ED%81%AC%EB%8B%89/)

### OllyDbg
Windows 환경에서 사용되는 32비트 어셈블리 레벨 분석 디버거입니다. 주로 리버스 엔지니어링, 악성코드 분석 등에 활용됩니다. 사용자 정의 플러그인을 지원하며, 강력한 분석 기능을 제공합니다. (현재는 개발이 중단되었으며, x64dbg와 같은 후속 도구들이 많이 사용됩니다.)
- **공식 사이트**: [http://www.ollydbg.de/](http://www.ollydbg.de/)

### SoftICE
과거 Windows 커널 디버깅에 강력한 기능을 제공했던 도구입니다. Windows XP 이후로는 공식적인 개발 지원이 중단되었지만, 시스템 프로그래밍 역사에서 중요한 위치를 차지했던 디버거입니다.

### WinDbg
Microsoft에서 제공하는 Windows용 디버거입니다. 사용자 모드 및 커널 모드 디버깅을 모두 지원하며, 드라이버 개발, 시스템 충돌 분석 등 고급 디버깅 작업에 필수적입니다. 강력하지만 사용법이 다소 복잡할 수 있습니다.
- **다운로드 및 정보**: [Debugging Tools for Windows (WinDbg)](https://docs.microsoft.com/en-us/windows-hardware/drivers/debugger/)

### IDA Pro
정적 및 동적 분석을 위한 강력한 디스어셈블러이자 디버거입니다. 주로 리버스 엔지니어링, 취약점 분석, 악성코드 분석 등 보안 분야에서 널리 사용됩니다. 다양한 프로세서 아키텍처와 파일 형식을 지원하며, Hex-Rays 디컴파일러와 같은 강력한 확장 기능을 통해 생산성을 높일 수 있습니다. 다만, 상용 소프트웨어로 라이선스 비용이 높은 편입니다.
- **공식 사이트**: [https://www.hex-rays.com/products/ida/](https://www.hex-rays.com/products/ida/)

### Intel Pin
Intel에서 개발한 동적 바이너리 계측(Dynamic Binary Instrumentation) 프레임워크입니다. 프로그램 실행 중에 코드를 삽입하거나 변경하여 프로그램의 동작을 분석하고 제어할 수 있게 해줍니다. 리버스 엔지니어링, 퍼징, 성능 분석, 테인트 분석 등 다양한 분야에 활용됩니다. 디버거 자체라기보다는 디버깅 도구나 분석 도구를 만드는 데 사용되는 강력한 도구입니다.
- **공식 사이트**: [Pin - A Dynamic Binary Instrumentation Tool](https://www.intel.com/content/www/us/en/developer/articles/tool/pin-a-dynamic-binary-instrumentation-tool.html)
- **관련 자료**:
  - [Taint Analysis 연구분석보고서 (teamcrak.tistory.com)](http://teamcrak.tistory.com/328)
  - [Dynamic Instrumentation Tool (KLDP)](https://kldp.org/node/112142)

{% include "templates/in-progress.md" %}
