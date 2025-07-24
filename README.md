아래는 요청하신 내용을 기반으로 작성한 `README.md` 파일입니다.
Windows 환경에서 **Rust + Bun + Tauri 기반의 Claudia 앱을 빌드하고 실행하는 전체 과정을 담았습니다.**

---

### 📄 `README.md`

````markdown
# Claudia App (Tauri + Bun + Rust)

Windows 환경에서 Rust, Bun, Tauri를 사용하여 `claudia` 앱을 설치, 빌드, 실행하는 방법입니다.

---

## 🦀 1. Rust 설치 (v1.70.0 이상)

1. [https://rustup.rs](https://rustup.rs) 에 접속
2. `rustup-init.exe` 다운로드 후 실행
3. 설치 마법사에서 [1] 기본 설치 진행

### ✅ 설치 확인
```bash
cargo --version
````

---

## 🥖 2. Bun 설치 (최신 버전)

```bash
npm install -g bun
```

> 📌 Node.js와 npm이 설치되어 있어야 합니다.
> [https://nodejs.org](https://nodejs.org)에서 LTS 버전 설치 권장

### ✅ 설치 확인

```bash
bun --version
```

---

## 📦 3. 프론트엔드 의존성 설치

프로젝트 디렉토리로 이동 후:

```bash
cd claudia
bun install
```

---

## 🛠 4. Production Build 실행파일 만들기

```bash
bun run tauri build
```

빌드가 완료되면 실행 파일이 아래 경로에 생성됩니다:

```
claudia\src-tauri\target\release\claudia.exe
```

---

## ▶ 5. 실행 파일 실행하기

1. 아래 경로로 이동:

```
claudia\src-tauri\target\release
```

2. `claudia.exe` 파일을 **우클릭 → 보내기 → 바탕화면에 바로가기 만들기**

3. 바탕화면에서 앱 실행 🎉

---

## 🧩 사용 기술

* [Rust](https://www.rust-lang.org/)
* [Bun](https://bun.sh/)
* [Tauri](https://tauri.app/)

```

---

이 파일을 `claudia` 폴더 안에 `README.md`로 저장하시면 됩니다.

필요하시면 제가 마크다운 파일로 생성해서 드릴 수도 있어요.  
원하시면 `.md` 파일 첨부해드릴게요!
```
