# Combat Vision Lab

對打運動影像分析模擬系統，支援拳擊、空手道、跆拳道與柔道的介面切換。

## 開啟

直接雙擊 `index.html`，或在此資料夾執行：

```bash
python3 -m http.server 8080
```

再開啟 `http://localhost:8080/`。

## 主要功能

- 四種運動專屬技術名稱、KPI、對比指標與場地視覺
- 明確的「匯入影片 → 開始分析 → 檢視結果」操作流程
- 按下「開始分析」後才啟動紅藍選手追蹤、骨架與軌跡模擬
- 下方 3D／俯視／側視動作分析，包含移動軌跡、速度曲線與事件時間軸
- 依拳擊、空手道、跆拳道、柔道切換不同的出拳、踢擊、投技與移動指標
- 本機影片匯入（影片保留在瀏覽器本機，不會自動上傳）
- 手動新增技術事件與 JSON 匯出
- 桌面、平板與手機響應式介面

## 測試影片

`test-videos/` 已放入拳擊、空手道、跆拳道與柔道各一支本機 MP4。開啟系統後先切換到對應運動，再按「匯入本機影片」選擇檔案：

- `test-videos/boxing-sparring.mp4`
- `test-videos/karate-sparring.mp4`
- `test-videos/taekwondo-sparring.mp4`
- `test-videos/judo-sparring.mp4`

完整作者、來源、授權與影片規格請見 `test-videos/SOURCES.md`。

## 重要限制

目前是互動介面與分析流程模擬，不含正式電腦視覺模型。畫面上的速度、距離、信心值與命中／得分資料均為模擬資料；必須完成場地比例、攝影機透視、影格率、動作標註及效度驗證後，才能作為正式量測依據。

製作單位：臺灣運動健康科技學會（Taiwan Society of Sports Health Technology，暫採中文名稱直譯）  
更新：2026 年 11 月（v0.2）

## 正式發布

- Firebase Hosting：`https://combat-vision-lab-skyfu218-v2.web.app`
- Hosting site：`combat-vision-lab-skyfu218-v2`
- Firebase project：`pulselens-fitness-skyfu218`
