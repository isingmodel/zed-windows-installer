# Zed Windows Installer

Zed 공식 Windows 설치 파일을 보관하는 비공식 미러입니다. Zed Industries와 제휴한 저장소가 아닙니다.

## 다운로드

**[Zed 1.27.0 Windows x64 설치 파일 다운로드](https://github.com/isingmodel/zed-windows-installer/raw/refs/heads/main/installers/Zed-x86_64.exe)**

| 항목 | 내용 |
| --- | --- |
| 버전 | 1.27.0 (Stable) |
| 공식 출시일 | 2026-11-04 |
| 보관일 | 2026-11-11 |
| 대상 | Windows x64 (Intel/AMD) |
| 파일 | `installers/Zed-x86_64.exe` |
| 크기 | 64,751,256 bytes (약 64.8 MB) |

다운로드한 `Zed-x86_64.exe`를 실행하고 설치 안내를 따르세요. ARM64 PC용 파일은 [Zed 공식 다운로드 페이지](https://zed.dev/download)에서 받을 수 있습니다.

## 무결성 확인

공식 GitHub 릴리스가 제공한 SHA-256:

```text
6a39f9a78a6aac805f5aedcf03384b4b49349e9282903f27ebafcb18dde538ca
```

Windows PowerShell에서 다음 명령으로 확인할 수 있습니다.

```powershell
Get-FileHash .\Zed-x86_64.exe -Algorithm SHA256
```

저장소를 복제한 경우 macOS/Linux에서는 `shasum -a 256 -c SHA256SUMS`로 확인할 수 있습니다.

## 출처와 소스 코드

- [공식 릴리스 v1.27.0](https://github.com/zed-industries/zed/releases/tag/v1.27.0)
- [공식 원본 설치 파일](https://github.com/zed-industries/zed/releases/download/v1.27.0/Zed-x86_64.exe)
- [해당 버전의 소스 코드와 빌드 자료](https://github.com/zed-industries/zed/tree/v1.27.0)
- [해당 버전의 소스 코드 ZIP 다운로드](https://github.com/zed-industries/zed/archive/refs/tags/v1.27.0.zip)
- [Windows 빌드 안내](https://github.com/zed-industries/zed/blob/v1.27.0/docs/src/development/windows.md)
- [공식 Windows 설치 안내](https://zed.dev/docs/windows)

설치 파일은 공식 배포본을 수정 없이 보관합니다. 이 저장소는 위에 명시한 버전을 보관하며 자동으로 업데이트하지 않습니다.

## 라이선스 및 고지

Zed의 저작권은 Zed Industries 및 해당 기여자에게 있습니다. 공식 소스는 주로 GPL-3.0-or-later이며, 표시된 일부 구성 요소는 Apache-2.0입니다. 해당 버전의 원본 라이선스를 [LICENSE-GPL](LICENSE-GPL), [LICENSE-APACHE](LICENSE-APACHE)에 포함했습니다.

제3자 구성 요소의 라이선스와 고지는 공식 배포본 및 [원본 소스의 라이선스 자료](https://github.com/zed-industries/zed/tree/v1.27.0/script/licenses)를 참조하세요. Zed 이름과 상표는 각각의 권리자에게 속합니다.
