# 🔄 SafeTalk – ユーザーフロー / User Flow / 사용자 흐름

---

## 🇯🇵 ユーザー行動の流れ

SafeTalkの利用は、以下のステップで構成されています：

1. 🔐 **ログイン / サインアップ**  
　ユーザーはメールやソーシャルアカウントでログインします。

2. 💬 **感情入力**  
　自由テキストを入力し、感情検出をリクエストします。

3. 📊 **感情分析結果の表示**  
　感情の種類（喜び、不安、怒りなど）と深刻度が視覚化されます。

4. 🤖 **GPTによるフィードバック提供**  
　分析結果に基づき、GPTが共感メッセージや行動ガイドを生成します。

5. 📁 **履歴保存 & オプション操作**  
　感情履歴がFirebaseに保存され、ユーザーは記録を見ることができます。

6. 🛎️ **通知 or 報告**（オプション）  
　深刻な場合はSlack / LINE通知を送信、またはユーザーが報告可能です。

---

## 🇺🇸 User Flow

The user experience in SafeTalk consists of the following steps:

1. 🔐 **Login / Sign-up**  
   Users log in via email or social accounts.

2. 💬 **Emotion Input**  
   Users enter free-form text and request emotion detection.

3. 📊 **Emotion Analysis Result**  
   The detected emotion type (e.g., joy, anxiety, anger) and severity are visualized.

4. 🤖 **GPT-based Feedback Generation**  
   Based on the result, GPT generates empathetic messages and suggested actions.

5. 📁 **History Saving & User Options**  
   The emotional history is stored in Firebase, and users can view previous records.

6. 🛎️ **Notification or Report (Optional)**  
   In severe cases, the system sends Slack/LINE alerts, or users can submit a report.

---

## 🇰🇷 사용자 흐름

SafeTalk은 다음과 같은 순서로 사용자 경험이 구성됩니다:

1. 🔐 **로그인 / 회원가입**  
   사용자는 이메일 또는 소셜 계정으로 로그인합니다.

2. 💬 **감정 입력**  
   자유롭게 텍스트를 입력하고 감정 분석을 요청합니다.

3. 📊 **감정 분석 결과 표시**  
   감정의 종류(예: 기쁨, 불안, 분노)와 심각도가 시각화되어 나타납니다.

4. 🤖 **GPT 피드백 제공**  
   분석 결과를 기반으로 GPT가 공감 메시지와 행동 제안을 생성합니다.

5. 📁 **감정 기록 저장 및 옵션**  
   감정 기록은 Firebase에 저장되며, 사용자는 이력을 열람할 수 있습니다.

6. 🛎️ **알림 전송 또는 신고 (선택 사항)**  
   심각한 경우 Slack / LINE 알림이 전송되거나 사용자가 직접 신고할 수 있습니다.