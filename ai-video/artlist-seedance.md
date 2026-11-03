# Artlist / Seedance 2.5 工作手冊

這份文件專門整理：
- Artlist 上使用 Seedance 2.5 的實戰規則
- 適合本專案的 Prompt 寫法
- 角色一致性控制
- 頭幀／尾幀規則
- 常見報錯與修正方式
- 適用於《絕區零》二創、遊戲 AI 劇場、真人 AI 短劇

## 1. 定位
Artlist 的 Seedance 2.5 是目前本專案的主力 AI 動畫生成工具。

### 主要用途
- 單鏡頭角色動作
- 遊戲角色二創動畫
- 情緒反應短片
- 短劇分鏡片段
- 首幀圖生影片
- 參考影片動作重演
- 頭幀／尾幀控制的短鏡頭

### 不適合直接期待
- 長篇完整劇情一次生成
- 多角色極複雜互動還要完全不跑掉
- 超高精度口型配音同步
- 完全不需要修正就直接出片

## 2. 核心原則
### 2.1 先圖後影
高風險鏡頭一律：
1. 先做頭幀
2. 確認角色臉、髮型、服裝、配件沒跑
3. 再拿去做影片

### 2.2 一幕只做一個主要動作
不要在同一段 Prompt 裡塞太多事。

### 2.3 臉一致優先於動作華麗
如果動作做大會讓臉崩掉，先保角色。

### 2.4 動作幅度要明講
Seedance 容易把動作做太小，可用：
- 快速
- 明顯
- 大幅度
- 猛地
- 立刻
- 明確地
- 用力地
- 瞬間

## 3. Prompt 固定結構
建議固定順序：
1. 主體是誰
2. 場景在哪
3. 景別 / 鏡位
4. 角色動作
5. 表情變化
6. 鏡頭運動
7. 光線 / 氣氛
8. 節奏
9. 必須保留的角色特徵
10. 禁止事項

## 4. 通用 Prompt 模板
### 4.1 單人動作
A single [character description] in [scene].  
[Shot size], [camera angle], [lens feeling].  
The character [main action in clear sequence].  
Facial expression: [expression].  
Camera movement: [push / pan / static / follow].  
Lighting: [lighting style].  
Pacing: [fast / medium / slow].  
Preserve the exact face, hairstyle, outfit colors, accessories, and body proportions.  
Do not change the character design.  
Do not add extra props.  
Do not change the clothing, hairstyle, or facial features.

### 4.2 雙人對話
Two characters in [scene].  
Character A stands [position], Character B stands [position].  
[Shot size], [camera angle].  
Character A [action / speaking reaction].  
Character B [reaction].  
Camera [movement].  
Keep both characters visually separate and consistent.  
Do not swap their positions.  
Do not mix their faces, hairstyles, outfits, accessories, or body proportions.

### 4.3 參考影片動作替換
Use the reference video only for motion, timing, camera movement, framing, and environment.  
Replace the original person with the target character.  
Preserve the exact pose flow, body movement, timing, and camera movement.  
Keep the target character’s face, hairstyle, outfit, colors, accessories, and body proportions unchanged.  
Do not add extra weapons or props unless explicitly requested.  
Do not change the environment unless explicitly requested.

## 5. 頭幀規則
### 5.1 目的
不是做最帥，而是做最穩定、最適合接下一個動作的起始姿勢。

### 5.2 頭幀檢查
- 五官清楚
- 髮型清楚
- 配色正確
- 衣服完整
- 配件正確
- 背景不要太亂
- 起手動作合理

### 5.3 道具動作
如果後續影片要「抽出手銬」，頭幀不要先亮手銬。  
應停在手準備往後腰伸或手搭在後腰附近。

## 6. 尾幀規則
適用於：
- 控制結尾姿勢
- 怕模型中途亂飄
- 固定最後表情
- 接下一幕

尾幀可控制：
- 最後視線
- 最後手部位置
- 是否抬手、拍手、震驚、崩潰
- 結尾定格

## 7. 角色一致性
優先順序：
1. 臉
2. 髮型
3. 服裝
4. 配件
5. 體型
6. 畫風
7. 場景

明確禁止：
- 不換臉
- 不美化
- 不改髮型
- 不改髮長
- 不改服裝
- 不改服裝配色
- 不加飾品
- 不改體型
- 不混其他角色特徵

多角色再加：
- 不交換前後景
- 不交換左右位置
- 不混臉
- 不混耳朵
- 不混尾巴
- 不混武器
- 不混服裝

## 8. 表情控制
不要只寫 angry / sad，要寫成可視覺化情緒，例如：
- 超嫌棄但壓著怒氣
- 勉強接受但非常疑惑
- 正常理解並尊重
- 開始有點小驚訝
- 明顯震驚
- 崩潰
- 徹底失控

### 眼神光
可用：
- eyes dull and lifeless
- eyes with only a faint glimmer
- eyes regain a little bit of light
- fully restored sparkle in the eyes

## 9. 鏡位與運鏡
景別：
- close-up
- medium close-up
- medium shot
- full body shot

機位：
- low angle
- eye level
- slightly high angle
- over-the-shoulder

運鏡：
- static shot
- slow push-in
- quick push-in
- slight handheld feel
- follow movement
- subtle pan

常用組合：
- 情緒反應：medium close-up + eye level + slow push-in
- 爆點動作：medium shot + slightly low angle + quick push-in
- 社死／尷尬：close-up + eye level + static / subtle push-in

## 10. 常見問題
### 10.1 動作太小
原因：
- 沒寫幅度
- 沒寫速度
- 沒寫起始與結束姿勢

修法：
- quickly reaches behind the waist
- forcefully pulls out the handcuffs
- raises them clearly into frame

### 10.2 臉跑掉
修法：
- 縮短片段
- 降低同段動作量
- 先做頭幀
- 強調 preserve the exact face

### 10.3 髮型／服裝亂改
加入：
- preserve the exact hairstyle and hair length
- preserve the exact outfit and color scheme
- do not redesign the costume

### 10.4 多角色混在一起
- 明講前景 / 後景 / 左 / 右
- 一次只讓一個角色做主要動作
- 加 do not swap positions

### 10.5 中文被翻英文
加入：
- only Traditional Chinese as spoken in Taiwan
- do not translate the dialogue
- do not rewrite the dialogue
- no English text
- no English speech

## 11. 保護內容／審核
若出現：
- This model can't generate content that may be protected.
- Image doesn't meet our guidelines.

修正方向：
- 改成描述角色外觀與職能
- 少寫官方專有名詞
- 聚焦動作、鏡頭、表情、構圖
- 有參考圖時，文字少重複點名 IP
- 高風險內容改成中性視覺描述

注意：不以規避平台安全規則為目標。

## 12. 實戰工作流
### 單鏡頭角色動畫
1. 定義角色與情緒
2. 先生成頭幀
3. 檢查臉與服裝
4. 寫 Seedance Prompt
5. 生成短片
6. 看哪裡跑掉
7. 再修 Prompt

### 參考影片替換角色
1. 提供參考影片
2. 提供角色參考圖
3. 指定誰替換誰
4. 保留動作 / 構圖 / 時間
5. 明寫不要混角色特徵
6. 分段做，不一次做完整長片

### 情緒連續短片
每幕先定義：
- 表情
- 眼神光
- 手勢
- 是否有道具
- 鏡頭距離

## 13. 建議輸出格式
每次寫 Seedance 2.5 Prompt 建議固定輸出：
1. 模型
2. 秒數
3. 是否需要頭幀
4. 完整 Prompt
5. 禁止事項
6. 失敗時備用改寫版

## 14. 建議秒數
- 情緒反應：3～5 秒
- 單一動作：4～6 秒
- 對話反應：3～4 秒
- 複合動作：拆成兩段，各 4～5 秒
- 不建議 8 秒以上塞很多複雜動作

## 15. 專案特別規則
### 使用者主力工具
- Artlist 上的 Seedance 2.5

### 使用者偏好
- 頭幀先做
- 臉一致最優先
- 不要換臉
- 不要亂改服裝
- 不要亂改髮型
- 中文台詞必須是台灣中文
- Prompt 要能直接複製
- 容易失敗時要提供較穩定改寫版

## 16. 維護方式
以下情況要更新本文件：
- 新 Seedance 報錯
- 某種 Prompt 特別有效
- 某種寫法特別容易失敗
- 某角色有固定容易跑掉的點
- Artlist 平台規則或功能變動
