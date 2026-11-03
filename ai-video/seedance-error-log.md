# Seedance 2.5 錯誤紀錄庫

這份檔案專門記：
- 發生什麼錯
- 當時 Prompt 怎麼寫
- 哪裡出問題
- 最後怎麼修
- 哪個修法有效

每次遇到新問題都追加，避免重複踩雷。

## 錯誤 001：動作幅度太小
### 症狀
角色只做很小的手部動作，沒有完成預期的大幅度動作。

### 常見原因
- 只寫「拿出」
- 沒寫速度
- 沒寫動作路徑
- 沒寫最後物件要出現在畫面中

### 有效修法
補上：
- quickly
- forcefully
- clearly
- large visible motion
- raises it fully into frame

### 結論
Seedance 對大動作最好寫成：
起點 → 動作 → 終點。

---

## 錯誤 002：臉跑掉
### 症狀
動作中角色臉型、眼睛、五官逐漸變形。

### 常見原因
- 動作太複雜
- 片段太長
- 運鏡太激烈
- 同時要求太多情緒變化

### 有效修法
- 縮短成 3～5 秒
- 一幕只做一個主要動作
- 先生成頭幀
- 加 preserve the exact face
- 減少強烈鏡頭旋轉

---

## 錯誤 003：髮型／髮長改變
### 症狀
短髮變長髮、髮束變形、瀏海改變。

### 有效修法
加入：
- preserve the exact hairstyle
- preserve the exact hair length
- do not redesign the hair

### 結論
髮長一定要獨立寫，不只寫 hairstyle。

---

## 錯誤 004：服裝／配色跑掉
### 症狀
衣服換款式、顏色變化、配件消失。

### 有效修法
加入：
- preserve the exact outfit
- preserve the exact color scheme
- preserve all accessories
- do not redesign the costume

---

## 錯誤 005：角色互換
### 症狀
前景角色變成背景角色，或左右位置交換。

### 有效修法
明寫：
- Character A stays in the left foreground
- Character B stays in the right background
- do not swap positions
- do not mix character identities

---

## 錯誤 006：多出武器／道具
### 症狀
背景角色突然多武器，或前景人物出現未指定配件。

### 有效修法
加入：
- do not add any weapon
- do not add any extra prop
- only keep the accessories visible in the reference image

---

## 錯誤 007：中文台詞被翻成英文
### 症狀
模型自動講英文或自動改寫中文。

### 有效修法
加入：
- only Traditional Chinese as spoken in Taiwan
- do not translate
- do not rewrite
- no English speech
- the dialogue must match exactly

---

## 錯誤 008：角色只剩局部身體
### 症狀
生成結果只剩雙腿、上半身消失或人物超出畫面。

### 常見原因
- crop / framing 指令不清楚
- 模型誤判角色位置
- 參考圖構圖太極端

### 有效修法
- 明寫 full upper body / full body visible
- 指定 character centered in frame
- 使用乾淨頭幀
- 避免過度 crop
- 先確認首幀構圖再生成

---

## 錯誤 009：不該碰的物件被互動
### 症狀
角色走向櫃子、碰櫃子、開抽屜。

### 有效修法
用否定句明寫：
- does not walk toward the cabinet
- does not touch the cabinet
- does not open any drawer
- remains in place

### 結論
「不要做」必須具體到動作層級。

---

## 錯誤 010：保護內容阻擋
### 症狀
出現：
This model can't generate content that may be protected.

### 可能原因
- 角色名／作品名太密集
- IP 參考描述過直接
- 參考圖與文字共同觸發保護

### 修正方向
- 聚焦視覺特徵、動作、鏡頭
- 減少重複 IP 名稱
- 有參考圖時，用「preserve the reference character」
- 不以規避安全機制為目標

---

## 錯誤 011：表情變化太突然
### 症狀
從無神直接跳成大笑或震驚，中間沒有過渡。

### 有效修法
把表情寫成階段：
1. dull
2. faint glimmer
3. slight realization
4. clear reaction

並加入：
- gradually
- subtly
- over the next few seconds

---

## 錯誤 012：動作太多導致畫面崩壞
### 症狀
角色同時轉身、跑、揮手、拿道具、鏡頭旋轉，最後全部跑掉。

### 有效修法
拆幕：
- 第一段只轉身
- 第二段只拿道具
- 第三段只做表情反應

### 結論
Seedance 短片不是「一段做完全部」，而是「一段做好一件事」。

---

# 錯誤紀錄模板

## 錯誤 XXX：名稱
### 症狀
-

### 原 Prompt 問題
-

### 修正方式
-

### 是否有效
- 有效 / 部分有效 / 無效

### 後續規則
-
