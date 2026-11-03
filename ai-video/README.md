# AI 動畫工具庫

這個區塊用來支援：
- 真人 AI 短劇
- 遊戲 AI 劇場
- 二次元角色動畫
- 圖生影片
- 動作轉移
- 角色一致性
- 對嘴
- Talking Head
- 多鏡頭短劇
- AI 配音＋字幕＋剪輯流程

## 使用原則
1. 先判斷需求，再選工具，不固定只用單一模型
2. 角色一致性優先於畫面華麗
3. 真人／二次元／遊戲角色要分開選工具
4. 能用參考圖就不用純文字硬猜
5. GitHub 收錄代表「納入工作流知識」，不等於目前環境一定已安裝


## 專案主力：Artlist / Seedance 2.5
目前使用者已有 Artlist AI 會員，Seedance 2.5 為 AI 動畫主力平台。

優先參考：
- `artlist-seedance.md`：Artlist / Seedance 2.5 主手冊
- `seedance-prompt-examples.md`：可複用 Prompt 範例
- `seedance-error-log.md`：錯誤與修正紀錄

### 選型原則
若 Artlist / Seedance 2.5 能完成需求，優先使用，不為了技術炫耀改用更複雜的自架模型。
只有當需求涉及 Seedance 明顯不擅長的功能，例如高精度對嘴、特定 motion transfer、自架批次流程時，再考慮其他工具。
