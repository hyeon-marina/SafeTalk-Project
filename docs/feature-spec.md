# 🧩 SafeTalk – 機能定義書 / Feature Specification / 기능 정의서

---

## 🇯🇵 SafeTalkの主な機能

以下は、SafeTalkにおけるコア機能とその説明です：

### 1. 感情分析（Emotion Detection）
- 📌 ユーザー入力のテキストから感情タイプ（喜び、不安、怒りなど）と深刻度を検出
- 🛠️ 独自モデルまたは外部APIと連携予定

### 2. GPTフィードバック生成（GPT Feedback）
- 📌 感情分析結果に基づいて、GPTが共感メッセージと行動ガイドを提供
- 🧠 メッセージは感情ごとにテンプレート制御＋AI 생성 병행

### 3. 感情履歴の可視化（Emotion History）
- 📌 過去の入力・感情・GPT応答を時系列で保存・表示
- 🔐 ユーザー別にFirebaseで管理

### 4. 多言語対応（Multilingual Support）
- 📌 日本語を基本に、英語・韓国語を対応
- 🌐 i18nextを使用し、自動検出とユーザー設定をサポート

### 5. 管理者通知機能（Admin Alert System）
- 📌 深刻な感情が検出された場合、SlackやLINEに通知を送信
- 🚨 通知条件と頻度は拡張可能

---

## 🇺🇸 Core Features of SafeTalk

Below are the core features of SafeTalk:

### 1. Emotion Detection
- 📌 Detects emotion type (joy, anxiety, anger, etc.) and severity from user input
- 🛠️ Integrated with custom models or external APIs

### 2. GPT Feedback Generation
- 📌 Provides empathetic messages and action guidance based on analysis results
- 🧠 Combines AI-generated text and controlled templates per emotion

### 3. Emotion History Visualization
- 📌 Stores and displays past inputs, emotional states, and GPT responses
- 🔐 Managed per user via Firebase

### 4. Multilingual Support
- 📌 Supports Japanese (default), English, and Korean
- 🌐 Uses i18next with auto-detection and manual switching

### 5. Admin Alert System
- 📌 Sends alerts via Slack or LINE if high-severity emotions are detected
- 🚨 Configurable rules and thresholds

---

## 🇰🇷 SafeTalk의 핵심 기능

아래는 SafeTalk에서 제공하는 주요 기능입니다:

### 1. 감정 분석
- 📌 사용자의 입력 텍스트로부터 감정 유형(기쁨, 불안, 분노 등)과 심각도를 분석합니다.
- 🛠️ 자체 모델 또는 외부 API와 연동 예정입니다.

### 2. GPT 피드백 생성
- 📌 감정 분석 결과에 따라 GPT가 공감 메시지 및 행동 가이드를 생성합니다.
- 🧠 감정별 템플릿 + AI 생성 메시지를 병행합니다.

### 3. 감정 이력 시각화
- 📌 사용자의 감정 및 GPT 응답 히스토리를 시간 순으로 저장하고 보여줍니다.
- 🔐 Firebase를 통해 사용자별로 안전하게 관리합니다.

### 4. 다국어 지원
- 📌 일본어를 기본으로 영어, 한국어까지 지원합니다.
- 🌐 i18next를 활용해 언어 자동 감지 및 수동 전환 기능을 제공합니다.

### 5. 관리자 알림 시스템
- 📌 심각한 감정이 탐지될 경우 Slack 또는 LINE으로 관리자에게 알림을 보냅니다.
- 🚨 조건과 빈도는 설정에 따라 조절 가능합니다.