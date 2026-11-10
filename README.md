# 도면 이미지 스튜디오 · Plan Image Studio

도면을 입력하고 **2D 평면도 / 3D 조감도 / 3D 완성 건물**을 생성하는 Windows 설치형 GUI입니다.

**VS Code OpenAI Codex의 ChatGPT OAuth 인증만 사용하며 API 키를 요구하지 않습니다.**

[최신 설치 파일 다운로드](https://github.com/ktk2480-dot/plan-image-studio-releases/releases/latest)

## 시작하기

1. Release에서 `PlanImageStudio-Setup-1.0.0-x64.exe`를 내려받아 설치합니다. Python을 별도로 설치할 필요가 없습니다.
2. VS Code의 OpenAI Codex 확장을 설치하고 ChatGPT 계정으로 로그인합니다. 앱의 로그인 버튼으로도 Codex OAuth를 시작할 수 있습니다.
3. 이미지 또는 PDF 도면을 불러옵니다. PDF는 페이지를 선택합니다.
4. 생성 유형을 고르고 추가 프롬프트를 입력합니다. 추가 프롬프트는 공란으로 두어도 됩니다.
5. **이미지 생성하기**를 누르면 유형에 맞는 프롬프트를 완성하여 Codex 내장 이미지 도구로 전달합니다.
6. 결과를 확대하거나 원본과 비교하고 이미지 파일로 저장합니다.

## 주요 기능

- PNG, JPG/JPEG, WEBP, BMP, TIFF 및 PDF 페이지 입력
- 2D 평면도, 내부가 보이는 3D 조감도, 지붕과 외벽이 갖춰진 3D 완성 건물
- 모드에 맞는 프롬프트 자동 완성 및 선택적인 추가 요청
- 원본·결과 비교, 확대·이동, PNG/JPEG/WEBP 저장
- 생성 기록 다시 열기와 작업 취소

## 실행 환경

- Windows 10/11, x64
- 내장 이미지 생성 기능을 지원하는 VS Code OpenAI Codex 확장
- Codex ChatGPT OAuth 로그인, 인터넷 및 해당 계정의 이미지 도구 사용 권한

이미지 생성에는 계정의 기능 제공 범위와 사용 한도가 적용됩니다. 도면에 없는 높이·지붕·외장 등은 추정 표현될 수 있습니다.

생성 결과와 입력 사본은 `%LOCALAPPDATA%\PlanImageStudio\jobs`에 보관합니다. 원본 파일은 수정하지 않습니다.

이 저장소는 **공개 설치 파일 배포용**입니다. 애플리케이션 소스는 별도 비공개 저장소에서 관리합니다. GitHub가 자동 제공하는 Source code ZIP에는 이 배포 저장소의 안내 문서만 들어 있습니다.

## 파일 확인

Release의 `SHA256SUMS.txt`에서 설치 파일의 SHA-256을 확인할 수 있습니다.

```powershell
Get-FileHash -Algorithm SHA256 .\PlanImageStudio-Setup-1.0.0-x64.exe
```

설치 파일은 코드 서명되지 않았습니다. 자세한 설치 안내는 Release의 `INSTALL.txt`를 확인해 주세요.
