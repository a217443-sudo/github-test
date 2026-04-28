# 公司介紹網站（GitHub Pages）

這個專案是靜態網站（`index.html`），已加入 **一鍵部署 GitHub Pages** 的工作流程。

## 一鍵部署（第一次只要做一次設定）

1. 到 GitHub 專案頁面 → **Settings** → **Pages**。
2. 在 **Build and deployment** 的 **Source** 選 **GitHub Actions**。
3. 回到專案首頁，點 **Actions** → **Deploy static site to GitHub Pages**。
4. 點 **Run workflow**，選 `main` 分支後執行。

完成後會得到公開網址：

- `https://a217443-sudo.github.io/Trandforce/`

## 之後更新網站（真正一鍵）

只要推送到 `main` 分支，就會自動重新部署：

```bash
git add .
git commit -m "update site"
git push origin main
```

工作流程檔案在：`.github/workflows/deploy-pages.yml`。
