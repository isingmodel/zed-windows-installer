# 파일 저장소

Zed와 OpenCode의 공식 배포 파일을 보관하는 비공식 미러입니다.

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

### Linux x86_64 원격 서버

**[Zed 1.27.0 Linux x86_64 원격 서버 다운로드](https://github.com/isingmodel/zed-windows-installer/raw/refs/heads/main/remote-server/zed-remote-server-linux-x86_64.gz)**

Linux x86_64 호스트에서 사용하는 원격 서버 파일입니다. 압축 파일의 크기는 약 39.2 MB입니다.

### OpenCode v2.2.7 Linux x64

`main` 브랜치에 약 61 MB씩 나눈 파일 2개를 보관합니다. 두 파일을 같은 폴더에 다운로드하세요.

[1번 파일](https://github.com/isingmodel/zed-windows-installer/raw/refs/heads/main/opencode/v2.2.7/opencode-linux-x64.tar.gz.part-01-of-02) · [2번 파일](https://github.com/isingmodel/zed-windows-installer/raw/refs/heads/main/opencode/v2.2.7/opencode-linux-x64.tar.gz.part-02-of-02)

다운로드한 폴더에서 다음 명령으로 원본 압축 파일을 복원하고 공식 SHA-256과 비교하세요.

```sh
cat opencode-linux-x64.tar.gz.part-01-of-02 opencode-linux-x64.tar.gz.part-02-of-02 > opencode-linux-x64.tar.gz
printf '%s\n' '89a6cee227b54bc011179c528a5e63176032462b1a5e21723b616801cddc2ca7  opencode-linux-x64.tar.gz' | sha256sum -c -
```

[분할 파일 폴더](opencode/v2.2.7) · [MIT 라이선스](opencode/v2.2.7/LICENSE-MIT.txt) · [OpenCode 공식 릴리스](https://github.com/anomalyco/opencode/releases/tag/v2.2.7)

## 무결성 확인

Zed 배포 파일의 공식 SHA-256은 [SHA256SUMS](SHA256SUMS)에서 확인할 수 있습니다. Windows 설치 파일의 SHA-256은 다음과 같습니다.

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
- [공식 원본 Linux x86_64 원격 서버 파일](https://github.com/zed-industries/zed/releases/download/v1.27.0/zed-remote-server-linux-x86_64.gz)
- [해당 버전의 소스 코드와 빌드 자료](https://github.com/zed-industries/zed/tree/v1.27.0)
- [해당 버전의 소스 코드 ZIP 다운로드](https://github.com/zed-industries/zed/archive/refs/tags/v1.27.0.zip)
- [Windows 빌드 안내](https://github.com/zed-industries/zed/blob/v1.27.0/docs/src/development/windows.md)
- [공식 Windows 설치 안내](https://zed.dev/docs/windows)

파일은 공식 배포본을 수정 없이 보관합니다. 이 저장소는 위에 명시한 버전을 보관하며 자동으로 업데이트하지 않습니다.

## 라이선스 및 고지

Zed의 저작권은 Zed Industries 및 해당 기여자에게 있습니다. 공식 소스는 주로 GPL-3.0-or-later이며, 표시된 일부 구성 요소는 Apache-2.0입니다. 해당 버전의 원본 라이선스를 [LICENSE-GPL](LICENSE-GPL), [LICENSE-APACHE](LICENSE-APACHE)에 포함했습니다.

제3자 구성 요소의 라이선스와 고지는 공식 배포본 및 [원본 소스의 라이선스 자료](https://github.com/zed-industries/zed/tree/v1.27.0/script/licenses)를 참조하세요. Zed 이름과 상표는 각각의 권리자에게 속합니다.
