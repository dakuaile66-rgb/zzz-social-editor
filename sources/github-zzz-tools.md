# GitHub —《絕區零》可用專案索引

這份清單只收「對社群內容、梗圖、角色研究、AI 二創、素材整理、資料自動化有實際用途」的 GitHub 專案。

> 原則：GitHub 專案是資料／工具來源，不代表內容一定正確或最新。角色名稱、版本劇情、社群熱梗仍需用官方與中文玩家社群交叉確認。

## 使用優先級

### P0 — 內容製作直接可用

#### Nagano-original-fireworks-store/Dimbreath-ZenlessData
- URL: https://github.com/Nagano-original-fireworks-store/Dimbreath-ZenlessData
- 類型：遊戲資料 dump
- 已確認 README：包含《絕區零》遊戲資料，TextMap 被獨立整理，方便以 key:value 方式查文字
- 用途：
  - 查遊戲內文字／名詞
  - 建立角色台詞與稱呼資料庫
  - 驗證文案是否嚴重 OOC
  - 未來可做角色／任務／文本搜尋
- 注意：屬非官方資料 dump；版本最新性要檢查
- 對本專案價值：★★★★★

#### mrfatworm/ZZZ-Archive
- URL: https://github.com/mrfatworm/ZZZ-Archive
- 類型：跨平台《絕區零》Wiki／資料瀏覽
- 已確認 README：支援繁體中文、iOS、Windows 等，整理遊戲資訊與熱門二創
- 用途：
  - 繁中角色／遊戲資料快速參考
  - UI／設計系統參考
  - 角色資料與二創題材輔助
- 注意：仍需跟官方最新版本交叉確認
- 對本專案價值：★★★★★

#### m4urlclo0/ZZZ-Assets
- URL: https://github.com/m4urlclo0/ZZZ-Assets
- 類型：《絕區零》Assets
- 用途：
  - 遊戲美術／角色素材結構研究
  - AI 生圖時建立「遊戲原畫 reference」概念
  - 視覺、材質、UI、角色比例參考
- 狀態：Archived
- 注意：
  - 不把它當最新版本素材來源
  - 素材使用需自行確認著作權／官方二創規範
- 對本專案價值：★★★★☆

#### bmjoy/ZZZStudio
- URL: https://github.com/bmjoy/ZZZStudio
- 類型：針對《絕區零》修改過的 AssetStudio
- 已確認 README：可建立 ZZZ Map、載入 bundle、匯出 asset list、模型／動畫等
- 用途：
  - 研究遊戲資產結構
  - 尋找模型／動畫／材質參考
  - 建立更準確的 AI 角色／場景 reference
- 注意：偏技術工具，不是梗圖生成器；避免拿來做未授權素材散布
- 對本專案價值：★★★★☆

#### DEViantUA/ZZZeroCard
- URL: https://github.com/DEViantUA/ZZZeroCard
- 類型：角色資訊卡生成 Python 模組
- 已確認 README：可由 HoYoLab／UID 資料建立角色卡
- 用途：
  - 做角色資訊卡型社群內容
  - 角色養成／玩家帳號視覺化
  - 延伸成「角色卡惡搞版」梗圖版型參考
- 注意：README 範例需 cookies；不要把私人 token／cookie 放進公開 repo
- 對本專案價值：★★★★☆

### P1 — 版本／活動／社群題材自動化

#### torikushiii/hoyoverse-api
- URL: https://github.com/torikushiii/hoyoverse-api
- 類型：HoYoverse REST API
- 已確認 README：《絕區零》支援兌換碼、活動日曆、卡池、News 等
- 可用語言包含中文參數
- 用途：
  - 自動抓版本活動
  - 卡池／活動時間提醒
  - 建立「現在版本能做什麼內容」的題材雷達
  - 未來接 n8n 自動化
- 注意：第三方 API；正式發布前仍需官方來源確認
- 對本專案價值：★★★★★

#### lgou2w/HoYo.Gacha
- URL: https://github.com/lgou2w/HoYo.Gacha
- 類型：米哈遊抽卡紀錄管理／分析
- 已確認 README：支援《原神》《星穹鐵道》《絕區零》，支援 UIGF、CSV
- 用途：
  - 抽卡統計內容
  - 「非／歐」玩家梗的真實資料支撐
  - 可把 CSV 接到 Google Sheet／分析流程
- 平台：README 目前主要列 Windows 10 x64+
- Mac 使用者：當成資料格式／流程參考，不預設本機可直接跑
- 對本專案價值：★★★★☆

#### JamXi233/ZenlessTools
- URL: https://github.com/JamXi233/ZenlessTools
- 類型：中文《絕區零》工具箱
- 已確認 README：帳號切換、多使用者抽卡分析
- 平台：Windows 10 x64／arm64
- 用途：
  - 了解中文玩家工具需求
  - 抽卡分析 UI／欄位設計參考
- Mac 使用者：不列為主力執行工具
- 對本專案價值：★★★☆☆

### P1 — 音樂／影音內容參考

#### marques-kevin/zenless-zone-zero-music.app
- URL: https://github.com/marques-kevin/zenless-zone-zero-music.app
- 類型：《絕區零》音樂播放器／音樂資料庫
- 已確認 README：可建立本地音樂庫與資料結構
- 用途：
  - 查找／整理 ZZZ 音樂題材
  - 剪輯配樂研究
  - 建立「角色／場景 → 適合 BGM」資料表
- 注意：音樂版權仍需依授權處理，GitHub 有資料不代表可任意商用
- 對本專案價值：★★★☆☆

#### marques-kevin/api.zenless-zone-zero-music.app
- URL: https://github.com/marques-kevin/api.zenless-zone-zero-music.app
- 類型：ZZZ Music API 後端
- 已確認 README：NestJS + PostgreSQL，支援 track、playlist、likes 等結構
- 用途：
  - 若未來自建音樂／素材資料庫，可參考 API 架構
  - 可借鑑 likes／playlist 欄位設計做內容素材管理
- 對本專案價值：★★★☆☆

### P2 — 可研究，但不是目前主力

#### OneDragon-Anything/ZenlessZoneZero-OneDragon
- URL: https://github.com/OneDragon-Anything/ZenlessZoneZero-OneDragon
- 類型：《絕區零》自動化工具
- 用途：了解玩家日常流程／介面辨識／自動化思路
- 本專案定位：僅研究，不作為梗圖／AI 生圖主工具
- 對本專案價值：★★☆☆☆

#### sMythicalBird/ZenlessZoneZero-Auto
- URL: https://github.com/sMythicalBird/ZenlessZoneZero-Auto
- 類型：《絕區零》自動化
- 用途：理解玩家高頻操作與日常痛點，可轉成題材研究
- 本專案定位：不直接整合遊戲自動操作
- 對本專案價值：★★☆☆☆

#### festivities/ZenlessLUT
- URL: https://github.com/festivities/ZenlessLUT
- 類型：ZZZ LUT／視覺相關專案
- 狀態：Archived
- 用途：研究《絕區零》色調／視覺處理方向
- 本專案定位：視覺參考，不當主力
- 對本專案價值：★★☆☆☆

## 不收進主工作流的類型

以下即使搜尋得到，也不列入「推薦可用工具」：
- Trainer／修改器
- 私服
- 作弊／繞過
- 只做遊戲逆向而跟內容製作無直接關係的工具
- 長期停止維護且無素材參考價值的專案

原因：對梗圖、短影音、角色資料、社群內容產出幫助低，還可能增加帳號／資安／使用條款風險。

## 對梗圖的正確用法

GitHub 資料不能直接告訴我們「現在什麼梗最好笑」。它負責的是：

1. **角色／台詞真實性**
   - ZenlessData
   - ZZZ-Archive

2. **遊戲畫風／素材 reference**
   - ZZZ-Assets
   - ZZZStudio

3. **版本／卡池／事件題材**
   - hoyoverse-api

4. **玩家真實數據梗**
   - HoYo.Gacha
   - ZenlessTools

5. **社群梗是否真的流行**
   - 仍以 X、NGA、B站／YouTube Shorts、Facebook、HoYoLAB 中文社群交叉確認

### 梗圖三種製作模式

#### A｜原遊戲截圖梗
- 優先級最高
- 用真實遊戲畫面／角色表情
- AI 只做必要修圖或排版
- AI 味最低

#### B｜原角色＋改情境
- 角色官方圖／遊戲截圖作 reference
- 鎖臉、髮型、服裝、配色、配件
- 改姿勢／場景／互動
- 適合「官方沒演，但玩家一看就懂」的惡趣味

#### C｜完全 AI 二創
- 只有 A/B 無法完成才用
- 必須有角色 reference + 遊戲 style reference
- 優先 IP-Adapter／LoRA／ControlNet 類工作流
- 不讓 AI 自己亂發明角色造型

## 內容安全規則
- 不把遊戲 dump 當成官方授權素材庫
- 不公開私人 cookie、token、UID 敏感資訊
- 不因 GitHub 有檔案就假設可商用
- 不把資料挖掘結果直接當官方已發布資訊
- 最新角色／版本／劇情以官方公開內容為準
