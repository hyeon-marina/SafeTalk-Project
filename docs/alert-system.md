# 🔔 SafeTalk – 通知システム構成 / Alert System Design / 알림 시스템 설계

> 📄 This document explains the alert system design used in SafeTalk,  
> focusing on how emotion severity triggers notifications via Slack and LINE Notify.

---

## 🇯🇵 通知設計（Slack / LINE）

SafeTalkでは、深刻な感情が検出された場合に、管理者に通知が送信されます。  
これにより、ユーザーの心理的危機に対して迅速な対応が可能となります。

### 🔹 通知条件（トリガー）

- 感情スコアが一定のしきい値（例：0.85以上）を超えた場合
- 「攻撃」「怒り」「絶望」などの高リスク感情タイプ
- ユーザーが「報告」ボタンを押下した場合（手動）

### 🔹 通知方法

| 種類 | 技術 | 用途 |
|------|------|------|
| Slack通知 | Incoming Webhook | 管理者チャンネルへ即時送信 |
| LINE通知 | LINE Notify API | 個人またはチーム管理者へ通知 |

### 🔹 メッセージ例（Slack）
```json
🚨 SafeTalk アラート発生
ユーザーID: anon_312
感情: 怒り (スコア: 0.91)
時間: 2025-06-01 15:32 JST
```

---

## 🇺🇸 Alert System (Slack / LINE Notify)

In SafeTalk, an alert is sent to administrators when a critical emotion is detected.  
This allows for timely intervention in potential psychological crises.

### 🔹 Notification Triggers

- Emotion severity score exceeds threshold (e.g., > 0.85)
- High-risk emotions such as "anger", "aggression", "despair"
- Manual reports from users via "Report" button

### 🔹 Notification Channels

| Type | Technology | Purpose |
|------|------------|---------|
| Slack | Incoming Webhook | Instant notification to admin channel |
| LINE | LINE Notify API | Alert to admin team or personal LINE |

### 🔹 Message Example (Slack)
```json
🚨 SafeTalk Alert Triggered
User ID: anon_312
Emotion: Anger (Score: 0.91)
Time: 2025-06-01 15:32 JST
```

---

## 🇰🇷 알림 시스템 설계 (Slack / LINE Notify)

SafeTalk에서는 심각한 감정이 감지되었을 때,  
관리자에게 즉시 알림을 보내는 시스템을 도입하고 있습니다.  
이로써 사용자의 위기 상황에 빠르게 대응할 수 있습니다.

### 🔹 알림 트리거 조건

- 감정 점수가 임계값(예: 0.85) 이상일 때
- "분노", "공격성", "절망" 등 위험 감정일 때
- 사용자가 직접 "신고" 버튼을 눌렀을 때

### 🔹 알림 수단

| 종류 | 기술 | 목적 |
|------|------|------|
| Slack | Incoming Webhook | 관리자 채널에 실시간 전송 |
| LINE | LINE Notify API | 개인 또는 팀 LINE으로 알림 전송 |

### 🔹 메시지 예시 (Slack)
```
🚨 SafeTalk 알림 발생
사용자 ID: anon_312
감정: 분노 (점수: 0.91)
시간: 2025-06-01 15:32 KST
```