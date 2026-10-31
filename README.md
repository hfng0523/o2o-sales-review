# O2O 銷售檢討 Dashboard

O2O 每日銷售檢討 dashboard（v4.1）：GMV / 訂單 / 客單價 / Discount Cost / ROI，
可按品類、會員、門市、AM、DM、星期拆解，附自動 insight 同門市升跌。

## 保安
- 全頁數據以 **AES-GCM 256-bit + PBKDF2-SHA256（200,000 iterations）** 加密
- 冇密碼 = 只見到密文，睇唔到任何銷售數據
- 密碼由 HKTVmall O2O Marketing 團隊保管

## 自動更新
每日 09:30（HKT）由 Hermes cron 抓最新 Tableau + PSOS 數據 → 重新加密 → 部署。
