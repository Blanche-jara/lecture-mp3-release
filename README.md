# 강의 MP3 다운로더

온라인 강의 영상을 MP3로 받고, 강의 화면을 캡처하고, 받아쓰기·교정·요약까지 하는 Windows 프로그램입니다.

**설명과 다운로드: https://pure-blanche.com/apps/lecture-mp3/**

이 저장소는 설치 파일을 배포하는 곳이며 소스 코드는 없습니다.
최신 버전은 [Releases](https://github.com/Blanche-jara/lecture-mp3-release/releases/latest)에서 받으세요.

## 파일

| 파일 | 설명 |
|------|------|
| `LectureMP3-Setup-<버전>.exe` | 설치 파일 (Windows 10/11 64비트) |
| `transcriber-<버전>.zip` | 받아쓰기 부품. 직접 받을 필요 없이, 프로그램이 필요할 때 받아서 확인한 뒤 설치합니다 |

## 설치

1. 설치 파일을 실행합니다. 관리자 권한은 필요 없습니다.
   "Windows의 PC 보호" 창이 뜨면 **추가 정보 → 실행**을 누르세요(코드 서명을 하지 않은 프로그램이라 뜹니다).
2. 쓸 기능을 고릅니다.
   - 받아쓰기(Whisper): 설치 후 부품 약 90MB, 첫 받아쓰기 때 음성인식 모델 약 1.6GB를 내려받습니다.
   - 교정·요약(Claude Code): Claude Pro 이상 요금제가 필요하고, 설치 후 로그인합니다.
3. 고르지 않은 기능은 나중에 프로그램의 **설정 → 기능 관리**에서 설치하거나 제거할 수 있습니다.

## 라이선스

- `tools/ffmpeg.exe`: FFmpeg 7.1 (gyan.dev essentials 빌드), GPLv3. 소스와 빌드 정보는 설치 폴더의
  `tools/FFMPEG-README.txt`에 있습니다.
- 함께 들어 있는 다른 소프트웨어의 라이선스: 설치 폴더의 `THIRD-PARTY-NOTICES.txt`와 `licenses` 폴더
  (받아쓰기 부품은 `components/transcriber` 안에 따로 있습니다).
