# 🌐 SafeTalk – 多言語対応構成 / Multilingual Structure / 다국어 처리 구조

> 📄 This document describes the i18n (internationalization) strategy used in SafeTalk,  
> including default language settings, folder structure, and key-value formatting for multilingual support.

---

## 🇯🇵 i18n設計方針（i18next）

SafeTalkは、i18nextライブラリを使用して、日本語、英語、韓国語の多言語対応を実現しています。

### 🔹 基本構成
- デフォルト言語：日本語
- ブラウザの言語設定により自動選択
- UIでの言語手動切替にも対応（ドロップダウン）

### 🔹 フォルダ構成（public/locales）
```json
public/
└── locales/
├── ja/
│   └── translation.json
├── en/
│   └── translation.json
└── ko/
└── translation.json
```

### 🔹 キー・値例（ja/translation.json）

```json
{
  "welcome": "SafeTalkへようこそ",
  "input_placeholder": "メッセージを入力してください",
  "analyzing": "感情を分析中...",
  "feedback_title": "AIからのフィードバック"
}
```
---

## 🇺🇸 i18n Design Strategy (i18next)

SafeTalk uses the i18next library to support multilingual interfaces (Japanese, English, Korean).

### 🔹 Structure Overview
	•	Default language: Japanese
	•	Automatically detects user language via browser
	•	Users can manually switch language via dropdown

### 🔹 Folder Structure
```json
public/
└── locales/
    ├── ja/
    │   └── translation.json
    ├── en/
    │   └── translation.json
    └── ko/
        └── translation.json
```

### 🔹 Key-Value Example (en/translation.json)
```json
{
  "welcome": "Welcome to SafeTalk",
  "input_placeholder": "Type your message...",
  "analyzing": "Analyzing your emotions...",
  "feedback_title": "Feedback from AI"
}
```

---

## 🇰🇷 i18n 설계 전략 (i18next 기반)

SafeTalk는 i18next 라이브러리를 활용해 일본어, 영어, 한국어 UI를 제공합니다.

### 🔹 핵심 설계
	•	기본 언어: 일본어
	•	브라우저 언어 자동 감지 및 설정
	•	드롭다운을 통해 언어 수동 전환 가능

### 🔹 폴더 구조
```json
public/
└── locales/
    ├── ja/
    │   └── translation.json
    ├── en/
    │   └── translation.json
    └── ko/
        └── translation.json
```

### 🔹 키-값 예시 (ko/translation.json)
```json
{
  "welcome": "SafeTalk에 오신 것을 환영합니다",
  "input_placeholder": "메시지를 입력하세요",
  "analyzing": "감정을 분석 중...",
  "feedback_title": "GPT 피드백"
}
```