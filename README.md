# sp9r

デスクトップアプリ、メディア処理パイプライン、データ可視化ツール、ブラウザ拡張機能、分割キーボード向けファームウェアなどの汎用ツールを開発・公開しています。

---

## 代表的な制作物（Featured Projects）

### 1. [flowpad](https://github.com/sp9r/flowpad) — Markdown・LaTeX ライブ描画対応の軽量タブ型メモ帳
**`C#` `.NET Framework 4.8` `WinForms` `WebView2` `KaTeX`**  
Windows標準メモ帳の軽快さと、カーソル移動に合わせたMarkdown・LaTeX数式（`$...$` / `$$...$$`）のその場でのライブレンダリングを両立したデスクトップメモアプリ。左右・上下の画面分割、タブドラッグによる別ウィンドウ切り離し・統合、文字コード自動判定・変換を備えています。

![Flowpad スクリーンショット](https://raw.githubusercontent.com/sp9r/flowpad/main/docs/screenshot.png)

---

### 2. [video_editor (Cutline)](https://github.com/sp9r/video_editor) & [clip_automation](https://github.com/sp9r/clip_automation) — 動画編集ソフト＆自動字幕・無音カットパイプライン
**`Electron` `TypeScript` `Python` `FFmpeg` `Whisper`**  
マルチトラックタイムライン・字幕スタイルテンプレート・自動無音カットを備えたデスクトップ動画編集アプリ（`video_editor`）と、音声認識・信号エネルギー解析による無音区間ジェットカット・字幕境界最適化を行うバックエンドパイプライン（`clip_automation`）。

---

### 3. [prefecture-cartogram](https://github.com/sp9r/prefecture-cartogram) — 都道府県別 連続面積カルトグラム
**`JavaScript` `TopoJSON` `Canvas / SVG`** （[GitHub Pages デモ](https://sp9r.github.io/prefecture-cartogram/)）  
都道府県ごとの統計データ（CSV）に応じて、日本地図の隣接関係（トポロジー）を保ったまま面積を連続変形させるインタラクティブ可視化ツール。

![都道府県別 連続カルトグラム](https://raw.githubusercontent.com/sp9r/prefecture-cartogram/main/docs/screenshot.png)

---

### 4. [PDF-editor](https://github.com/sp9r/PDF-editor) — PDFページ編集GUI＆PDF→PowerPoint変換ツール
**`Python` `PyMuPDF` `Tkinter` `python-pptx`**  
PyMuPDFによるサムネイルプレビューを確認しながらページ削除・並べ替え・回転を行えるGUIツールと、スライド構成を保ったPDF→PowerPoint変換スクリプト。

---

### 5. [keyball44-layer6-jis](https://github.com/sp9r/keyball44-layer6-jis) — Keyball44 VIA 6レイヤー＆JIS配列対応QMKファームウェア
**`C` `QMK Firmware` `Docker` `VIA`**  
分割トラックボールキーボード Keyball44 でVIAのキーマップを6レイヤー化し、JIS配列と組み合わせるためのQMKファームウェアおよび再現ビルド環境。

---

## 公開リポジトリ一覧

### デスクトップ・メディア・PDF処理
- **[flowpad](https://github.com/sp9r/flowpad)**: Markdown / LaTeX リアルタイム描画・画面分割・複数ウィンドウ対応の軽量タブ型メモ帳（C# .NET Framework 4.8 WinForms + WebView2）
- **[video_editor](https://github.com/sp9r/video_editor)**: Cutline — タイムライン編集・字幕テンプレート・自動無音カット対応の動画編集ソフト（Electron + TypeScript）
- **[clip_automation](https://github.com/sp9r/clip_automation)**: 音声認識・無音カット・字幕境界最適化パイプライン（Python + WebUI）
- **[PDF-editor](https://github.com/sp9r/PDF-editor)**: PyMuPDFプレビュー付きPDFページ編集GUIツール＆PDF→PowerPoint変換スクリプト

### Webツール・データ可視化
- **[prefecture-cartogram](https://github.com/sp9r/prefecture-cartogram)**: 都道府県別データの連続面積カルトグラム可視化（[Demo](https://sp9r.github.io/prefecture-cartogram/)）
- **[PWmaker](https://github.com/sp9r/PWmaker)**: Web Crypto API（CSPRNG）を用いた安全なランダム文字列・パスワード生成ツール（[Demo](https://sp9r.github.io/PWmaker/)）
- **[Caesar-cipher](https://github.com/sp9r/Caesar-cipher)**: Web Crypto API（AES-256-GCM + PBKDF2）によるブラウザ完結テキスト暗号化ツール（[Demo](https://sp9r.github.io/Caesar-cipher/)）

### ブラウザ拡張機能
- **[browser-extensions](https://github.com/sp9r/browser-extensions)**: 自作Chrome拡張機能コレクション（タブ切替時自動PiP、X数値非表示、YouTube秒単位投稿時刻、Amazon×バリューブックス在庫価格比較）
- **[YTmusicKeepAwake](https://github.com/sp9r/YTmusicKeepAwake)**: YouTube Musicの無操作時自動停止を防ぐChrome拡張機能
- **[HideOwnTweet](https://github.com/sp9r/HideOwnTweet)**: X（旧Twitter）上で自分の投稿・リプライを一時非表示にするChrome / Firefox拡張機能
- **[Gemini-search](https://github.com/sp9r/Gemini-search)**: URLクエリパラメータからGeminiへ直接質問を送るブラウザ拡張機能

### ハードウェア・ファームウェア
- **[keyball44-layer6-jis](https://github.com/sp9r/keyball44-layer6-jis)**: 分割キーボード Keyball44 のVIA 6レイヤー拡張＆JIS配列対応QMKファームウェア・Dockerビルド環境
