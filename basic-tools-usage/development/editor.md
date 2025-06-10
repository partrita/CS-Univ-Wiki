# 코드 에디터 및 통합 개발 환경 (IDE)

코드 에디터와 통합 개발 환경(IDE)은 프로그래머가 소스 코드를 작성하고 편집하는 데 사용하는 기본적인 소프트웨어입니다. 효율적인 코딩, 디버깅, 프로젝트 관리를 위해 적절한 도구를 선택하는 것이 중요합니다.

## 에디터의 종류

### 1. 터미널 기반 에디터
주로 서버 환경이나 커맨드 라인 인터페이스(CLI)에서 작업할 때 사용됩니다. 가볍고 빠르며, 키보드 중심으로 작업을 수행하는 데 특화되어 있습니다.

#### Vim (Vi IMproved)
Vi 에디터에서派생된 강력한 텍스트 에디터입니다. 다양한 운영체제에서 사용할 수 있으며, 수많은 단축키와 모드(일반, 입력, 비주얼 등)를 활용하여 효율적인 텍스트 편집이 가능합니다.
- **특징**: 높은 학습 곡선을 가지고 있지만, 익숙해지면 매우 생산적인 작업이 가능합니다. `.vimrc` 설정 파일을 통해 개인화할 수 있으며, 방대한 플러그인 생태계(예: Vundle, Vim Awesome)를 통해 기능을 확장할 수 있습니다.
- **학습 자료**: [OpenVim](http://www.openvim.com/) (인터랙티브 튜토리얼), [Vim Cheat Sheet](http://www.worldtimzone.com/res/vi.html)
- **팁**: NeoVim은 Vim을 현대적으로 개선한 프로젝트로, 더 나은 기본 설정과 확장성을 제공합니다. `ctags`나 `gtags`와 같은 도구와 연동하여 코드 탐색 기능을 강화할 수 있습니다.

#### Emacs (GNU Emacs)
Vim과 함께 터미널 기반 에디터의 양대 산맥으로 불립니다. Lisp 프로그래밍 언어를 통해 고도로 확장 가능하며, 단순한 텍스트 편집기를 넘어선 하나의 작업 환경으로 사용되기도 합니다 (예: 이메일, 파일 관리, 웹 브라우징 등).
- **특징**: Vim과 마찬가지로 학습 곡선이 있지만, 강력한 확장성과 사용자 정의 기능을 제공합니다.

#### Nano
간단하고 사용하기 쉬운 터미널 기반 에디터입니다. Vi나 Emacs보다 기능은 적지만, 직관적인 단축키(화면 하단에 표시됨)를 제공하여 초보자도 쉽게 사용할 수 있습니다. 간단한 설정 파일 수정 등에 유용합니다.
- **팁**: 대부분의 Linux 배포판에 기본적으로 포함되어 있으며, 문법 강조 기능을 지원합니다.

### 2. GUI 텍스트 에디터
그래픽 사용자 인터페이스(GUI)를 제공하여 마우스 사용이 가능하고, 시각적으로 더 친숙한 환경에서 코드를 편집할 수 있게 해줍니다. 많은 GUI 에디터들이 플러그인이나 확장 기능을 통해 IDE와 유사한 기능을 제공하기도 합니다.

#### Visual Studio Code (VS Code)
Microsoft에서 개발한 무료 오픈소스 코드 에디터입니다. 가볍고 빠르면서도 강력한 기능을 제공하여 현재 가장 인기 있는 에디터 중 하나입니다.
- **특징**: 다양한 프로그래밍 언어 지원, IntelliSense (자동 완성, 코드 제안), 디버깅 기능, Git 통합, 방대한 확장 기능 마켓플레이스.
- **공식 사이트**: [https://code.visualstudio.com/](https://code.visualstudio.com/)

#### Sublime Text
빠른 속도와 강력한 편집 기능, 사용자 정의 기능을 제공하는 상용 코드 에디터입니다 (무료 평가판 사용 가능). "Goto Anything", 다중 선택, 커맨드 팔레트 등의 기능이 특징입니다.
- **특징**: 다양한 패키지(플러그인)를 통해 기능을 확장할 수 있습니다 ([Package Control](https://packagecontrol.io/)).
- **공식 사이트**: [https://www.sublimetext.com/](https://www.sublimetext.com/)

#### Atom
GitHub에서 개발한 무료 오픈소스 코드 에디터입니다. Electron 프레임워크를 기반으로 하며, 웹 기술(HTML, CSS, JavaScript)을 사용하여 에디터 자체를 커스터마이징할 수 있습니다.
- **특징**: Git 통합, 다양한 패키지 및 테마 지원. VS Code와 유사한 부분이 많으나, 최근에는 VS Code의 사용 빈도가 더 높은 경향이 있습니다.
- **공식 사이트**: [https://atom.io/](https://atom.io/)

#### EditPlus
Windows 환경에서 사용되는 가볍고 빠른 텍스트 에디터입니다. 간단한 코드 편집이나 웹 개발에 사용되며, FTP 기능 등을 내장하고 있습니다.

### 3. 통합 개발 환경 (IDE - Integrated Development Environment)
코드 편집기, 컴파일러, 디버거, 빌드 자동화 도구 등 소프트웨어 개발에 필요한 여러 기능들을 하나로 통합하여 제공하는 환경입니다. 대규모 프로젝트나 특정 플랫폼 개발에 유용합니다.

#### Visual Studio
Microsoft에서 개발한 강력한 IDE입니다. Windows 애플리케이션, .NET 개발, C++ 게임 개발 등에 널리 사용됩니다. 풍부한 기능과 디버깅 도구를 제공합니다.
- **공식 사이트**: [https://visualstudio.microsoft.com/](https://visualstudio.microsoft.com/)

#### JetBrains IDEs (IntelliJ IDEA, PyCharm, CLion, etc.)
JetBrains사에서 개발한 다양한 언어 및 플랫폼별 IDE 제품군입니다. 강력한 코드 분석, 리팩토링, 자동 완성 기능으로 유명합니다.
- **PyCharm**: Python 개발용 IDE
- **IntelliJ IDEA**: Java 개발용 IDE (Community 버전 무료, Ultimate 버전 유료)
- **CLion**: C/C++ 개발용 IDE. Linux 환경에서 Visual Studio 대안으로 많이 사용됩니다.
- **기타**: WebStorm (JavaScript), PhpStorm (PHP), GoLand (Go), Android Studio (Android, IntelliJ 기반) 등
- **특징**: 대부분 유료이지만, 학생에게는 무료 교육용 라이선스를 제공하는 경우가 많습니다. ([JetBrains 학생 라이선스](https://www.jetbrains.com/student/))

#### Eclipse
주로 Java 개발에 사용되는 오픈소스 IDE입니다. 플러그인 아키텍처를 통해 C/C++, PHP 등 다양한 언어를 지원하도록 확장할 수 있습니다.
- **공식 사이트**: [https://www.eclipse.org/](https://www.eclipse.org/)

#### Android Studio
Google에서 공식적으로 제공하는 Android 앱 개발용 IDE입니다. IntelliJ IDEA를 기반으로 하며, Android 개발에 필요한 모든 도구와 기능을 통합 제공합니다.
- **공식 사이트**: [https://developer.android.com/studio](https://developer.android.com/studio)

## 선택 가이드
- **간단한 스크립트나 설정 파일 편집**: Nano, 가벼운 GUI 에디터
- **웹 프론트엔드 개발**: VS Code, Sublime Text, Atom
- **서버 환경에서의 작업**: Vim, Emacs
- **특정 언어/플랫폼 기반의 대규모 프로젝트**: 해당 언어/플랫폼에 특화된 IDE (예: Java - IntelliJ/Eclipse, Python - PyCharm, C/C++ - Visual Studio/CLion)

자신의 작업 환경, 주로 사용하는 언어, 프로젝트의 규모, 개인적인 선호도 등을 고려하여 적합한 도구를 선택하고 익숙해지는 것이 중요합니다.

{% include "templates/in-progress.md" %}
