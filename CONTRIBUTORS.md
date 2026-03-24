# 組員貢獻紀錄

> 完成自己的分支後，把名字和任務狀態填進來，送出 PR。
> 這個檔案大家都要修改，會產生 Merge Conflict——這是刻意設計的！

---

## 第 X 組

| 角色 | 姓名 | 負責分支 | 任務 | 狀態 |
|------|------|---------|------|------|
| 組長 | （填名字）| `main` | 修改標題 & header 顏色、review 所有 PR | ⬜ |
| 組員 A | （填名字）| `feature/member-a` | 新增訊息時間戳 | ⬜ |
| 組員 B | （填名字）| `feature/member-b` | 新增清除對話按鈕 | ⬜ |
| 組員 C | （填名字）| `feature/member-c` | 新增字數統計 | ⬜ |
| 組員 D | （填名字）| `feature/member-d` | 新增深色模式 | ⬜ |
| 組員 E | （填名字）| `feature/member-e` | 新增鍵盤快捷鍵說明 | ⬜ |

狀態：⬜ 未開始 / 🔄 進行中 / ✅ 已完成 / 🔀 PR 已開 / ✔️ 已 Merge

---

## 各組員任務說明

### 組長（`main` branch）
- [ ] 把 `index.html` 裡「第 X 組」改成實際組名
- [ ] 修改 `style.css` 裡 `header` 的背景顏色
- [ ] 填入所有組員姓名
- [ ] 設定 Branch Protection（Settings → Branches → Require PR + **2 approvals**）
- [ ] Review 每個 PR，留下至少 1 條有意義的 comment
- [ ] Merge 所有 PR（按順序：A → B → C → D → E，解決 conflict）

### 組員 A（`feature/member-a` branch）
- [ ] 在 `sendMessage()` 裡，每則訊息加上時間戳（`HH:MM` 格式）
- [ ] 在 `style.css` 加上 `.timestamp` 樣式（小字、靠右、半透明）
- [ ] 填寫完整 PR 描述（做了什麼 / 如何測試）
- [ ] 收到 2 位成員 review 後回應 comment
- [ ] Review 其他組員的 PR（至少 2 個）

### 組員 B（`feature/member-b` branch）
- [ ] 在 `index.html` 的 `.input-area` 加入「清除」按鈕
- [ ] 在 `<script>` 加入 `clearChat()` 函數，清空 `#chat-box`
- [ ] 在 `style.css` 加上清除按鈕的樣式（與送出按鈕顏色不同）
- [ ] 填寫完整 PR 描述
- [ ] 收到 2 位成員 review 後回應 comment
- [ ] Review 其他組員的 PR（至少 2 個）

### 組員 C（`feature/member-c` branch）
- [ ] 在 `index.html` header 下方加字數統計（「已輸入 X 字」）
- [ ] 在 `user-input` 的 `oninput` 事件更新字數
- [ ] 在 `style.css` 加上字數統計的樣式
- [ ] 填寫完整 PR 描述
- [ ] 收到 2 位成員 review 後回應 comment
- [ ] Review 其他組員的 PR（至少 2 個）

### 組員 D（`feature/member-d` branch）
- [ ] 在 header 加深色模式切換按鈕（`🌙`）
- [ ] 在 `style.css` 加上 `body.dark` 相關樣式
- [ ] 在 `<script>` 加上切換函數
- [ ] 填寫完整 PR 描述
- [ ] 收到 2 位成員 review 後回應 comment
- [ ] Review 其他組員的 PR（至少 2 個）

### 組員 E（`feature/member-e` branch）
- [ ] 在 `<footer>` 加入鍵盤快捷鍵說明（Enter 送出 / Esc 清空）
- [ ] 在 `<script>` 加入 Esc 清空輸入框的監聽
- [ ] 在 `style.css` 補 footer 樣式
- [ ] 填寫完整 PR 描述
- [ ] 收到 2 位成員 review 後回應 comment
- [ ] Review 其他組員的 PR（至少 2 個）

---

## 預期會出現的 Conflict

組員 A、B、C、D、E 都會修改 `index.html` 和 `style.css`。

合併時一定會出現 conflict——這是刻意設計的，練習解決！
