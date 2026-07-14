# 大長腿來闖關｜英文五大句型

一個給小朋友練習英文「五大基本句型」的網頁小遊戲。看句子，判斷它屬於哪一種句型，答完立刻顯示正解與句子拆解（S / V / O / C / IO / DO）。

- 題庫共 200＋ 題，五種句型各 40 句，另含第四型「換句話說」變體
- 每次隨機抽 20 題，五大句型混合出題
- 可勾選只練某幾種句型
- 答對綠色、答錯紅色，即時回饋不重複計分
- 最佳成績存在瀏覽器（localStorage）

## 五大句型（依波羅英文編號）

| 句型 | 結構 | 例句 |
|------|------|------|
| 1 | S + V | She laughs. |
| 2 | S + V + O | I love you. |
| 3 | S + V + C | He is cute. |
| 4 | S + V + IO + DO | He gave me a pencil. |
| 5 | S + V + O + C | You made me sad. |

## 直接使用

用瀏覽器打開 `index.html` 即可，不需要安裝任何東西、也不需要伺服器。

## 用 GitHub Pages 發佈（免費上線）

1. 在 GitHub 建立一個新的 repository（例如 `sentence-patterns`），設為 Public。
2. 把 `index.html` 和 `README.md` 上傳到這個 repo 的根目錄。
3. 進入 repo 的 **Settings → Pages**。
4. 在 **Build and deployment → Source** 選 **Deploy from a branch**。
5. Branch 選 `main`、資料夾選 `/ (root)`，按 **Save**。
6. 等一兩分鐘，頁面上方會出現網址，格式為：
   `https://<你的帳號>.github.io/sentence-patterns/`
   打開就能玩，也能直接分享給別人。

> 之後只要更新 `index.html` 再 push，網站會自動重新部署。

## 用指令上傳（如果你習慣命令列）

```bash
# 在放著 index.html 的資料夾裡
git init
git add index.html README.md
git commit -m "初版：英文五大句型闖關"
git branch -M main
git remote add origin https://github.com/<你的帳號>/sentence-patterns.git
git push -u origin main
```

推上去後，再依上面的步驟到 Settings → Pages 開啟即可。

## 技術說明

- 單一 HTML 檔，內含 CSS 與原生 JavaScript，無任何外部相依套件
- 純前端、純靜態，適合 GitHub Pages / Netlify / Cloudflare Pages 等任何靜態託管
