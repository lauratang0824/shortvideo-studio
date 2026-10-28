# 短影音工坊

上傳影片或圖片素材、選擇範本、填寫主題標題與字幕，就能在瀏覽器內自動剪出短影音並下載。

整個工具放在 GitHub 上：網頁由 GitHub Pages 提供，團隊共用的範本存在 `data/templates.json`，範本用到的配樂和 Logo 存在 `data/assets/`。素材影片只在使用者自己的瀏覽器裡處理，不會上傳。

## 使用方式

- **做影片（任何人）：** 打開網頁 →「生成影片」→ 選範本 → 上傳素材 → 填標題與字幕 → 生成影片 → 下載。建議使用電腦版 Chrome 或 Edge，可以輸出 MP4。
- **新增或修改範本（需要編輯權限）：** 到「範本管理」按「啟用編輯權限」，貼上自己的 GitHub 權杖。

## 讓同事可以編輯範本

1. 在這個儲存庫的 Settings → Collaborators 把同事加進來（需要 Write 權限）。
2. 同事建立自己的權杖：GitHub → Settings → Developer settings → Fine-grained tokens → Generate new token。
   - Repository access：Only select repositories，選這個儲存庫
   - Permissions → Contents：Read and write
3. 在網頁「範本管理」→「啟用編輯權限」貼上權杖。權杖只存在那台電腦的瀏覽器。

儲存範本後，其他人大約 1 分鐘後會看到更新（GitHub Pages 需要時間重新發布）。

## 注意

- 免費版 GitHub Pages 需要儲存庫設為 **Public**，範本設定、配樂和 Logo 檔案是公開可讀的。素材影片不會上傳，不受影響。
- 配樂與 Logo 單檔上限 20 MB。
- 範本資料就是 `data/templates.json`，可以直接在 GitHub 上編輯或備份。
