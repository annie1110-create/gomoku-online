# 🎮 正式五子棋 Online

一個實時多人五子棋遊戲，使用 Firebase 即時數據庫作為後端。

## 功能特點

✅ **正式15×15棋盤** - 符合國際五子棋規格  
✅ **星位標記** - 標準棋盤星位  
✅ **即時對戰** - 使用 Firebase 實現實時同步  
✅ **房間系統** - 支持建立和加入遊戲房間  
✅ **響應式設計** - 支持桌面和手機裝置  
✅ **自動勝負判定** - 任意方向5連珠自動判勝  

## 安裝步驟

1. **下載或複製此倉庫**

2. **配置 Firebase**
   - 訪問 [Firebase Console](https://console.firebase.google.com/)
   - 建立新項目
   - 啟用 Realtime Database
   - 複製你的 Firebase 配置信息
   - 在 `config.js` 中填入你的 Firebase 配置：

```javascript
const FIREBASE_CONFIG = {
  apiKey: "你的APIKEY",
  authDomain: "你的authDomain",
  databaseURL: "你的databaseURL",
  projectId: "你的projectId",
  storageBucket: "你的storageBucket",
  messagingSenderId: "你的messagingSenderId",
  appId: "你的appId"
};
```

3. **打開遊戲**
   - 直接在瀏覽器中打開 `index.html`
   - 或使用本地伺服器（推薦）

## 使用說明

### 建立房間
1. 輸入你的玩家名稱
2. 點擊 **建立房間** 按鈕
3. 系統會生成一個房號
4. 分享房號給對手

### 加入房間
1. 輸入你的玩家名稱
2. 在 **房號** 欄位輸入房間代碼
3. 點擊 **加入房間** 按鈕
4. 等待遊戲開始

### 遊戲規則
- 黑棋先手
- 玩家輪流在棋盤交叉點上放置棋子
- 任意方向（橫、豎、斜）連成5顆或以上棋子即獲勝
- 點擊 **重新開始** 按鈕開始新遊戲

## 技術棧

- **前端**: HTML5, CSS3, Vanilla JavaScript
- **後端**: Firebase Realtime Database
- **網路**: WebSocket (Firebase 內置)

## 瀏覽器支持

- Chrome/Chromium 最新版本
- Firefox 最新版本
- Safari 最新版本
- Edge 最新版本

## 文件結構

```
gomoku-online/
├── index.html      # 主遊戲文件
├── config.js       # Firebase 配置
└── README.md       # 說明文檔
```

## 許可證

MIT

## 聯繫方式

如有問題或建議，歡迎提交 Issue 或 Pull Request！
