# 第五週 Pull Request 協作練習

這是第五週的分組作業，練習完整的 Pull Request 協作流程。
**重點不只是寫程式，而是 PR 描述、Code Review 與回應 review 的過程。**

---

## 基本資料

| 項目        | 填寫           |
| ----------- | -------------- |
| 組別        | 第 ＿ 組       |
| 組員        |                |
| GitHub Repo |                |
| 報告日期    | 2025 / ＿ / ＿ |

---

## 快速開始

**組長**

1. Fork 該 repo → 命名為 `w5-collab-第X組` → **Create fork**
2. Settings → Branches → Add rule：`main`，勾選 **Require PR + 2 approvals**
3. Settings → Collaborators → 邀請所有組員
4. 把 repo URL 告訴組員

**組員**

```bash
git clone https://github.com/組長帳號/w5-collab-第X組.git
cd w5-collab-第X組
git checkout -b feature/member-a   # 依角色選擇
```

---

## Review Comment 範例

每個 PR 至少需要 **2 位成員 approve** 才能 merge。
Review 時留下有意義的 comment，以下是常見的寫法：

**✅ 肯定 / Approve 常用語**

```
LGTM!
```

```
LGTM! 邏輯很清楚，merge 沒問題 👍
```

```
Ship it! 🚀
```

```
Nice work! 時間戳格式選得很好，HH:MM 簡潔又夠用。
```

```
Looks good to me, 就這樣 merge 吧。
```

**💬 提問或確認意圖**

```
nit: 這個變數名稱可以再清楚一點嗎？（nit = nitpick，小建議，不影響 approve）
```

```
Esc 清空是清空輸入框還是整個對話？PR 描述可以補一下。
```

```
這裡用 querySelectorAll 是有考慮到未來擴充嗎？好奇問一下 😄
```

```
optional: 可以加 localStorage 記住 dark mode 狀態，但不一定要這次做。
```

**🔧 建議修改**

```
nit: `d` 這個變數名不太好懂，建議改成 `chatBox`。
```

```
這裡有重複的程式碼，可以抽成一個 function，會更好維護。
```

```
minor: clearChat 沒有 confirm 視窗，使用者可能會不小心清掉，要不要加個確認？
```

**⚠️ 指出問題（Request changes）**

```
這裡如果輸入是空字串會壞掉，需要先加個判斷再 merge。
```

```
WIP? 這個 function 好像還沒實作完，先確認一下？
```

```
blocking: 這個會影響其他功能，需要修一下才能 merge。
```

---

**常見縮寫對照**

| 縮寫     | 全文               | 意思               |
| -------- | ------------------ | ------------------ |
| LGTM     | Looks Good To Me   | 沒問題，可以 merge |
| nit      | Nitpick            | 小建議，不強制修改 |
| WIP      | Work In Progress   | 還沒做完           |
| PTAL     | Please Take A Look | 請幫我看一下       |
| TBD      | To Be Determined   | 待確認             |
| optional | —                 | 可做可不做的建議   |
| blocking | —                 | 必須修才能 merge   |

> **記住**：review 是討論，不是批判。指出問題時說明原因，建議修改方向，而不是直接否定。

---

## PR 描述規範（每個 PR 都要填）

```markdown
## 做了什麼
- （說明新增或修改了什麼）

## 如何測試
1. （步驟一）
2. （步驟二）

## 截圖
（附上修改後的畫面截圖）
```

---

## 完整協作流程

```
組長：Fork 模板 → 設 Branch Protection → 邀請組員
  ↓
各組員：clone → 建分支 → 完成任務 → push → 開 PR（填完整描述）
  ↓
組長：Review PR → 留 comment → Approve
  ↓
組員：回應 comment → 修改 → re-push
  ↓
組長：Merge（解決 conflict）
  ↓
全組：git pull origin main → 確認成果
```

---

## 一、協作分工

| 組員姓名 | 負責分支 | 主要修改內容 | PR 連結 | 是否完成 |
| -------- | -------- | ------------ | ------- | -------- |
|          |          |              |         | ✅ / ❌  |
|          |          |              |         | ✅ / ❌  |
|          |          |              |         | ✅ / ❌  |
|          |          |              |         | ✅ / ❌  |
|          |          |              |         | ✅ / ❌  |

---

## 二、截圖紀錄

### 2-1 PR 列表截圖（必填）

> 截圖：GitHub repo → Pull requests，顯示所有 PR 的狀態（open / merged）

（貼上截圖）

---

### 2-2 PR 描述截圖（必填）

> 截圖：其中一個 PR 的描述頁面，顯示完整的「做了什麼 / 如何測試」內容

（貼上截圖）

---

### 2-3 Code Review 截圖（必填）

> 截圖：Files changed 頁面，顯示 inline comment 的留言

（貼上截圖）

---

### 2-4 Merge 成功截圖（必填）

> 截圖：某個 PR 頁面顯示「Merged」紫色標籤

（貼上截圖）

---

### 2-5 最終成果截圖（必填）

> 截圖：用瀏覽器打開 `index.html`，顯示所有功能整合完成的畫面

（貼上截圖）

---

## 三、遇到的問題與解決方式

**問題 1：**

解決方式：

---

**問題 2：**

解決方式：

---

## 四、個人心得

> 每位組員各寫 2–3 句，說明這週對 PR / Code Review 的理解或感想

**（組員姓名）：**

**（組員姓名）：**

**（組員姓名）：**

---

## 五、自評與互評

| 評分項目            | 分數（1–5） | 說明 |
| ------------------- | ------------ | ---- |
| PR 描述完整度       |              |      |
| Review comment 品質 |              |      |
| 回應 review 的態度  |              |      |
| 最終成果完整度      |              |      |

這週覺得最有挑戰的是？

- [ ] 寫 PR 描述
- [ ] 給 Code Review
- [ ] 回應 review 並修改
- [ ] 解決 Merge Conflict
- [ ] 其他：＿＿＿

---

*報告由全組共同完成，commit 到 main 後繳交。*
