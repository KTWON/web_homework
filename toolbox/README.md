# 數據檢驗工具箱

以統計方法檢驗資料特性的線上工具集，透過 GitHub Pages 架設。所有計算都在瀏覽器中完成，不需要伺服器。

## 目前的工具

| 工具 | 路徑 | 說明 |
|---|---|---|
| 班佛定律檢驗器 | `benford/` | 檢驗第一、第二位數是否符合班佛定律，含適用性檢查與分析報告 |

## 資料夾結構

```
├── index.html          首頁（工具清單）
├── 404.html            找不到頁面時顯示
├── .nojekyll           讓 GitHub Pages 直接提供靜態檔案，不經過 Jekyll 處理
└── benford/
    └── index.html      班佛定律檢驗器
```

## 新增一個工具

1. 建立新資料夾，例如 `newtool/`，把工具頁面命名為 `index.html` 放進去。
2. 在新頁面加上回首頁的連結：`<a href="../">← 回到工具箱首頁</a>`。
3. 打開根目錄的 `index.html`，找到 `const TOOLS = [`，在陣列中加一筆：

   ```js
   ,{ title:'新工具名稱', tag:'分類', desc:'一句話說明', href:'newtool/' }
   ```

4. 視需要調整 `const PLACEHOLDERS = 2;`，控制首頁顯示幾張「即將推出」的預留卡片（設為 0 即不顯示）。
5. 上傳（commit）後，約 1 分鐘 GitHub Pages 會自動更新。

## 網址

- 首頁：`https://<你的帳號>.github.io/<儲存庫名稱>/`
- 班佛定律檢驗器：`https://<你的帳號>.github.io/<儲存庫名稱>/benford/`
