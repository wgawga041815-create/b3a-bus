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

## 資料來源

- 城巴開放數據（DATA.GOV.HK）：`https://rt.data.gov.hk/v2/transport/citybus/`
- 使用 `route-stop` 與 `eta` 端點；到站時間為預計，僅供參考。
- 本專案與城巴、DATA.GOV.HK 無官方關係。

## 圖片與版權

- 首頁角色圖選用《青春ブタ野郎》電視動畫官方網站（ao-buta.com）的櫻島麻衣主視覺，經裁切及調色後使用。
- 角色圖片版權歸原作者／製作委員會所有；本專案為非商業、非官方粉絲作品。
- 如版權持有人要求，會立即移除相關圖片。

## 技術

- `index.html`：單頁，內嵌 CSS/JavaScript，不需要 build step
- `mai-hero.jpg`：首頁主視覺
- `og.jpg`：分享預覽圖
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
