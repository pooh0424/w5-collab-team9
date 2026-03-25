# 組員貢獻紀錄

> 完成自己的分支後，把名字和任務狀態填進來，送出 PR。
> 這個檔案大家都要修改，會產生 Merge Conflict——這是刻意設計的！

---

## 第九組

| 角色 | 姓名 | 負責分支 | 任務 | 狀態 |
|------|------|---------|------|------|
| 組長 | 呂紹銘| `main` | 修改標題 & header 顏色、review 所有 PR | ✅ |
| 組員 A | 曹世杰 | `feature/member-a` | 新增訊息時間戳 | ⬜ |
| 組員 B | 林楷祐 | `feature/member-b` | 新增清除對話按鈕 |✅ |

狀態：⬜ 未開始 / 🔄 進行中 / ✅ 已完成 / 🔀 PR 已開 / ✔️ 已 Merge

---

## 各組員任務說明

### 組長（`main` branch）
- [x] 把 `index.html` 裡「第 X 組」改成實際組名
- [x] 修改 `style.css` 裡 `header` 的背景顏色
- [x] 填入所有組員姓名
- [x] 設定 Branch Protection（Settings → Branches → Require PR + **2 approvals**）
- [ ] Review 每個 PR，留下至少 1 條有意義的 comment
- [ ] Merge 所有 PR（按順序：A → B，解決 conflict）

### 組員 A（`feature/member-a` branch）
- [ ] 在 `sendMessage()` 裡，每則訊息加上時間戳（`HH:MM` 格式）
- [ ] 在 `style.css` 加上 `.timestamp` 樣式（小字、靠右、半透明）
- [ ] 填寫完整 PR 描述（做了什麼 / 如何測試）
- [ ] 收到 2 位成員 review 後回應 comment
- [ ] Review 其他組員的 PR（至少 2 個）

### 組員 B（`feature/member-b` branch）
- [x] 在 `index.html` 的 `.input-area` 加入「清除」按鈕
- [x] 在 `<script>` 加入 `clearChat()` 函數，清空 `#chat-box`
- [x] 在 `style.css` 加上清除按鈕的樣式（與送出按鈕顏色不同）
- [ ] 填寫完整 PR 描述
- [ ] 收到 2 位成員 review 後回應 comment
- [ ] Review 其他組員的 PR（至少 2 個）

---

## 預期會出現的 Conflict

組員 A、B 都會修改 `index.html` 和 `style.css`。

合併時一定會出現 conflict——這是刻意設計的，練習解決！
