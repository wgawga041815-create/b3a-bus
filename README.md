# B3A 實時到站看板

香港城巴 **B3A**（山景邨 ↔ 深圳灣口岸）的實時到站看板，為手機而設，每 30 秒自動更新。

**網址：** https://wgawga041815-create.github.io/b3a-bus/

## 功能

- 兩個方向：往深圳灣口岸、往山景邨
- 可選擇沿線任何可上車的站；選擇會記住（localStorage）
- 顯示下一班、第 2 班、第 3 班的預計到站時間
- 每 30 秒自動更新，亦可手動更新
- 手機優先的深色介面，無外部字體、無圖片、無追蹤

## 資料來源

- 城巴開放數據（DATA.GOV.HK）：`https://rt.data.gov.hk/v2/transport/citybus/`
- 使用 `route-stop` 與 `eta` 端點；到站時間為預計，僅供參考。
- 本專案與城巴、DATA.GOV.HK 無官方關係。

## 技術

單一 `index.html`（內嵌 CSS/JavaScript）＋ `favicon.svg`，不需要 build step，直接由 GitHub Pages 提供。

## 更新

修改 `index.html` 後：

```bash
git add index.html
git commit -m "Update board"
git push
```

GitHub Pages 會在一分鐘內重新部署。
