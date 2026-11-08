# sp9r

普段の生活や学習の中で感じた不便や「これがあったら便利なのに」を、電子工作（マイコン・回路）からデスクトップアプリ、Webバックエンド、ブラウザ拡張機能まで自分で設計・実装して日常運用しています。

---

## 代表的な制作物（Featured Projects）

### 1. [campus-hub](https://github.com/sp9r/campus-hub) — 履修・課題・教材 統合ローカルポータル
**`Python` `FastAPI` `SQLite` `Docker` `JavaScript`**  
別々に分かれている学務情報システム（KOAN）と学習管理システム（CLE / Blackboard）、シラバス、学事暦を1つの高速なローカル画面に統合するWebワークスペース。SAML SSO + TOTP自動認証で差分同期し、時間割から講義資料のインラインPDFプレビュー・課題提出確認・休講/補講の自動反映まで一気通貫で行えます。

![Campus Hub ホーム画面](https://raw.githubusercontent.com/sp9r/campus-hub/main/docs/screenshots/home-light.png)

---

### 2. [flowpad](https://github.com/sp9r/flowpad) — Markdown・LaTeX ライブ描画対応の軽量タブ型メモ帳
**`C#` `.NET 8` `WPF` `WebView2` `KaTeX`**  
Windows標準メモ帳の軽快さと、カーソル移動に合わせたMarkdown・LaTeX数式（`$...$` / `$$...$$`）のその場でのライブレンダリングを両立したデスクトップメモアプリ。講義ノートや数式メモをストレスなく記述できます。

![Flowpad スクリーンショット](https://raw.githubusercontent.com/sp9r/flowpad/main/docs/screenshot.png)

---

### 3. [doorbell-microbit](https://github.com/sp9r/doorbell-microbit) — インターホン呼出信号の分圧検知 × 家中通知システム
**`micro:bit` `ESP32-S3 (ATOMS3 Lite)` `TypeScript` `C++` `Raspberry Pi` `ntfy`**  
室内インターホン親機（NAiS SHN6200WK）の空き増設スピーカー端子から呼出信号（AC 1.1V）を抵抗分圧＋中点バイアス回路で取り出し、マイコンのADCで振幅を検知してRaspberry Pi（ntfy）経由で家中のPC・Chromebook・スマートフォンへリアルタイム通知・チャイム鳴動を行うハードウェア連携システム。

---

### 4. [video_editor (Cutline)](https://github.com/sp9r/video_editor) & [clip_automation](https://github.com/sp9r/clip_automation) — 動画編集ソフト＆自動字幕・無音カットパイプライン
**`Electron` `TypeScript` `Python` `FFmpeg` `Whisper`**  
マルチトラックタイムライン・字幕スタイルテンプレート・自動無音カットを備えたデスクトップ動画編集アプリ（`video_editor`）と、音声認識・信号エネルギー解析による無音区間ジェットカット・字幕境界最適化を行うバックエンドパイプライン（`clip_automation`）。

---

### 5. [kakeibo](https://github.com/sp9r/kakeibo) — 実質残高・カード引落予約・外貨ウォレット対応のローカル家計簿
**`Python` `Flask` `SQLite` `JavaScript`**  
クレジットカード利用分を「決済時点で差し引いた実質残高」として計算し、毎月の固定費予約枠・外貨ウォレット・Excel家計簿インポート・メール通知取込を備えたローカルWeb家計簿アプリ。

![Kakeibo スクリーンショット](https://raw.githubusercontent.com/sp9r/kakeibo/main/docs/screenshot.png)

---

### 6. [prefecture-cartogram](https://github.com/sp9r/prefecture-cartogram) — 都道府県別 連続面積カルトグラム
**`JavaScript` `TopoJSON` `Canvas / SVG`** （[GitHub Pages デモ](https://sp9r.github.io/prefecture-cartogram/)）  
都道府県ごとの統計データ（CSV）に応じて、日本地図の隣接関係（トポロジー）を保ったまま面積を連続変形させるインタラクティブ可視化ツール。

![都道府県別 連続カルトグラム](https://raw.githubusercontent.com/sp9r/prefecture-cartogram/main/docs/screenshot.png)

---

## カテゴリ別の公開リポジトリ一覧

### ハードウェア・IoT・スマートホーム連携
- **[doorbell-microbit](https://github.com/sp9r/doorbell-microbit)**: インターホン呼出信号の分圧検知 × micro:bit / ATOMS3 Lite × Raspberry Pi（ntfy）通知システム
- **[smartplus-hub](https://github.com/sp9r/smartplus-hub)**: マンションのスマートインターホン（SmartPlus）をローカルで一元管理するWebハブ・OpenAPI・Python SDK
- **[cz1-frame](https://github.com/sp9r/cz1-frame)**: postmarketOSを導入したChromebook（ASUS CZ1）をPCからWeb制御する情報パネル・サブディスプレイシステム
- **[keyball44-layer6-jis](https://github.com/sp9r/keyball44-layer6-jis)**: 分割キーボード Keyball44 のVIA 6レイヤー拡張＆JIS配列対応QMKファームウェア・Dockerビルド環境

### デスクトップ・メディア・生活アプリ
- **[flowpad](https://github.com/sp9r/flowpad)**: Markdown / LaTeX リアルタイム描画対応の軽量タブ型メモ帳（C# WPF + WebView2）
- **[video_editor](https://github.com/sp9r/video_editor)**: Cutline — タイムライン編集・字幕テンプレート・自動無音カット対応の動画編集ソフト（Electron + TypeScript）
- **[clip_automation](https://github.com/sp9r/clip_automation)**: 音声認識・無音カット・字幕境界最適化パイプライン（Python + WebUI）
- **[kakeibo](https://github.com/sp9r/kakeibo)**: 実質残高・固定費予約枠・外貨ウォレット・Excel連携対応のローカル家計簿Webアプリ（Flask + SQLite）
- **[PDF-editor](https://github.com/sp9r/PDF-editor)**: PyMuPDFプレビュー付きPDFページ編集GUIツール＆PDF→PowerPoint変換スクリプト

### 学習・スケジュール・自動化ツール
- **[campus-hub](https://github.com/sp9r/campus-hub)**: 学務システム（KOAN）× LMS（CLE）× シラバス統合ローカルポータル（FastAPI + Docker）
- **[koan-client](https://github.com/sp9r/koan-client)**: KOAN HTTP/SAML/TOTP自動ログインCLI・ライブラリ
- **[zoom-auto-record](https://github.com/sp9r/zoom-auto-record)**: Zoom会議プロセス検知＋OBS自動録画・ファイル名変更スクリプト
- **[Enhancer-for-OU](https://github.com/sp9r/Enhancer-for-OU)**: 学内Webシステム（KOAN / CLE / 認証画面）の操作性を高めるChrome拡張機能
- **[AutoClassroomLINE](https://github.com/sp9r/AutoClassroomLINE)**: Google Classroomの通知を解析してLINEへ自動転送するスクリプト

### Webツール・ブラウザ拡張機能
- **[prefecture-cartogram](https://github.com/sp9r/prefecture-cartogram)**: 都道府県別データの連続面積カルトグラム可視化（[Demo](https://sp9r.github.io/prefecture-cartogram/)）
- **[browser-extensions](https://github.com/sp9r/browser-extensions)**: 自作Chrome拡張機能コレクション（タブ切替時自動PiP、X数値非表示、YouTube秒単位投稿時刻、Amazon×バリューブックス在庫価格比較）
- **[YTmusicKeepAwake](https://github.com/sp9r/YTmusicKeepAwake)**: YouTube Musicの無操作時自動停止を防ぐChrome拡張機能
- **[HideOwnTweet](https://github.com/sp9r/HideOwnTweet)**: X（旧Twitter）上で自分の投稿・リプライを一時非表示にするChrome / Firefox拡張機能
- **[Gemini-search](https://github.com/sp9r/Gemini-search)**: URLクエリパラメータからGeminiへ直接質問を送るブラウザ拡張機能
- **[mood-tracker](https://github.com/sp9r/mood-tracker)**: Tailwind CSS + Chart.js による気分記録・推移可視化Webアプリ（[Demo](https://sp9r.github.io/mood-tracker/)）
- **[PWmaker](https://github.com/sp9r/PWmaker)**: Web Crypto API（CSPRNG）を用いた安全なランダム文字列・パスワード生成ツール（[Demo](https://sp9r.github.io/PWmaker/)）
- **[Caesar-cipher](https://github.com/sp9r/Caesar-cipher)**: Web Crypto API（AES-256-GCM + PBKDF2）によるブラウザ完結テキスト暗号化ツール（[Demo](https://sp9r.github.io/Caesar-cipher/)）
