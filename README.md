# 🧱 Tetris

<p align="center">
C++20 표준과 객체 지향 프로그래밍(OOP)을 활용하여 개발된 터미널 기반 테트리스
게임입니다.
</p>

## 💻 Screenshot

[image](./res/git/screenshot1.png)

## ✨ Features & Tech Stack

- 객체 지향 설계: 테트리스 블록(Tetromino), 보드(Board), 게임 로직 등 핵심 요소를 C++ 클래스로 구현하여 모듈화와 재사용성을 높였습니다.

- C++20 표준: 최신 C++ 를 활용하여 코드를 작성했습니다.

- 빌드 유연성: 필요에 따라 최적화 플래그(-O2, -g2 등)를 변경할 수 있습니다.

## 🚀 Build & Run

⚠️ 중요: 이 프로젝트는 Windows 운영 체제 환경에서만 빌드 및 실행이 가능하도록
구성되었습니다.

#### 최적화 플래그 변경 (Optimization Flag)

Makefile 내에서 빌드 시 적용할 최적화 플래그를 자유롭게 변경할 수 있습니다.

```makefile
# 기본 설정 예시 (디버깅)
FLAGS=-std=c++20 -g2 -Wall -Wextra -Werror -o $(TARGET)
# 상용 릴리즈 예시 (최적화)
FLAGS=-std=c++20 -O2 -Wall -Wextra -Werror -o $(TARGET)
```

#### 1. 빌드 (Build)

프로젝트 루트 디렉터리에서 make 명령어를 사용하여 빌드합니다.

```bash
# 기본 빌드
make all
```

#### 2. 실행 (Execution)

빌드 후 생성된 실행 파일을 실행합니다.

```bash
./tetris.exe
```

#### 3. Makefile 명령어

| 명령어 | 설명 |
| :--- | :--- |
| `make all` | 프로젝트를 빌드합니다. |
| `make re` | 모든 빌드 결과물을 정리(`clean`)한 후 다시 빌드합니다. |
| `make clean` | 컴파일된 모든 바이너리 파일 및 결과물을 제거합니다. |

## 🎮 Controls

게임 조작은 키보드의 방향키와 주요 키를 사용합니다.

| 입력 키 | 동작 |
| :--- | :--- |
| **↑ (방향키 상)** | 블록 회전 (Rotate) |
| **← (방향키 좌)** | 블록 왼쪽 이동 (Move Left) |
| **→ (방향키 우)** | 블록 오른쪽 이동 (Move Right) |
| **↓ (방향키 하)** | 블록 아래로 이동 (Move Down) |
| **Space Bar / Enter** | 블록 즉시 하강 (Hard Drop) |
| **Esc** | 일시 정지 메뉴 호출 (Pause Menu) |

## 📄 라이선스 (License)

이 프로젝트는 MIT 라이선스를 따릅니다.
