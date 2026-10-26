# B3A 實時到站看板 · 桜島麻衣主題

香港城巴 **B3A**（山景邨 ↔ 深圳灣口岸）的實時到站看板，為手機而設，每 30 秒自動更新。

**網址：** https://wgawga041815-create.github.io/b3a-bus/

## 功能

- 兩個方向：往深圳灣口岸、往山景邨
- 預設上落車站：**富泰邨**（往深圳灣口岸）、**富泰商場**（往山景邨），兩站均近嶺南大學
- 可選擇沿線任何車站（終點站除外）；選擇會記住（localStorage）
- 顯示下一班、第 2 班、第 3 班的預計到站時間
- 每 30 秒自動更新，亦可手動更新
- 手機優先的深色／櫻花介面，分享按鈕、無追蹤
- 人物圖片暫時移除，現以兔耳 B3A、櫻花配色與每日寄語呈現

## 資料來源與連線

- 城巴開放數據（DATA.GOV.HK）：`https://rt.data.gov.hk/v2/transport/citybus/`
- 使用 `route-stop` 與 `eta` 端點；到站時間為預計，僅供參考。
- 若主網域被代理／VPN 攔截，頁面會自動改用同一 API 的 CloudFront 端點（`d3amutxzdzfxs.cloudfront.net`）。
- 本專案與城巴、DATA.GOV.HK 無官方關係。

## 技術

- `index.html`：單頁，內嵌 CSS/JavaScript，不需要 build step
- `favicon.svg`：兔耳 B3A 圖示

直接由 GitHub Pages 提供。

## 更新

修改 `index.html` 後：

```bash
git add index.html
git commit -m "Update board"
git push
```

GitHub Pages 會在一分鐘內重新部署。
