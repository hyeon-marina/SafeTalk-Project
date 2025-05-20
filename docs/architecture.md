# 🛠️ SafeTalk – アーキテクチャ / System Architecture / 시스템 아키텍처

---

## 🇯🇵 技術構成とシステム全体像

SafeTalkは、以下の構成要素で構築されています：

### 🔹 フロントエンド (Frontend)
- 使用技術：React, TypeScript, TailwindCSS
- ユーザーインターフェースの表示、感情入力画面、GPTフィードバックの表示などを担当

### 🔹 バックエンド (Backend)
- 使用技術：FastAPI (Python)
- フロントからの感情分析・GPT応答リクエストを処理
- Firebaseとの連携も担当

### 🔹 AI・感情分析・GPT (AI Layer)
- OpenAI GPT API を使用してフィードバック生成
- 独自の感情分類モデル（例：BERT, SVMなど）で感情タイプと深刻度を推定

### 🔹 データベース・認証 (Auth/DB)
- Firebase Authentication：ログイン機能
- Firestore：感情履歴の保存・参照

### 🔹 外部通知サービス (External Notification)
- Slack Webhook / LINE Notify API：深刻なケースの通知を管理者に送信

---

## 🇺🇸 System Overview and Architecture

SafeTalk consists of the following technical components:

### 🔹 Frontend
- **Tech stack**: React, TypeScript, TailwindCSS  
- Handles UI rendering, emotion input screen, and GPT feedback display

### 🔹 Backend
- **Tech stack**: FastAPI (Python)  
- Receives requests from the frontend, triggers emotion analysis & GPT response  
- Connects with Firebase

### 🔹 AI Layer
- **OpenAI GPT API**: Generates empathetic responses  
- **Custom emotion classifier**: Estimates emotion type and severity (e.g., BERT/SVM)

### 🔹 Auth & Database
- **Firebase Auth**: User login and authentication  
- **Firestore**: Stores and retrieves emotional history

### 🔹 External Notification
- **Slack Webhook / LINE Notify API**: Sends alerts to administrators in critical cases

---

## 🇰🇷 시스템 구성 및 기술 구조 설명

SafeTalk는 다음과 같은 주요 기술 요소들로 구성되어 있습니다:

### 🔹 프론트엔드
- **기술 스택**: React, TypeScript, TailwindCSS  
- 사용자 UI, 감정 입력창, GPT 피드백 화면 등을 구현합니다.

### 🔹 백엔드
- **기술 스택**: FastAPI (Python)  
- 프론트엔드 요청을 받아 감정 분석 및 GPT 응답 처리를 수행하며, Firebase와의 연동도 담당합니다.

### 🔹 AI 계층
- **OpenAI GPT API**: 공감 기반 응답 생성  
- **자체 감정 분류 모델**: 감정 종류 및 심각도 예측 (예: BERT, SVM)

### 🔹 인증 및 데이터베이스
- **Firebase 인증**: 사용자 로그인 처리  
- **Firestore**: 감정 분석 결과 및 이력 저장/조회

### 🔹 외부 알림 시스템
- **Slack Webhook / LINE Notify API**: 심각한 상황에서 관리자에게 알림 전송