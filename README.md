# PChome API Scraper (Lightweight)

[![Python Version](https://img.shields.io/badge/python-3.7%2B-blue)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

這是一個高效能的 Python 爬蟲腳本，專門用於爬取 PChome 搜尋結果。與傳統使用 Selenium 模擬瀏覽器的方法不同，本專案透過直接呼叫 PChome 內部 API 獲取資料，具有極快的執行速度與低資源消耗。

## 📖 專案背景
在網頁爬蟲領域，直接分析 **Reverse Engineered API (逆向 API)** 的效率遠高於解析 HTML。本專案透過分析 PChome v4.3 API，跳過網頁渲染過程，直接取得結構化的 JSON 資料。

## ✨ 功能亮點
- **極致速度**：無需啟動 Chrome 瀏覽器，執行效率提升約 10-20 倍。
- **純淨資料**：僅提取 `Name` (名稱)、`Describe` (描述)、`Price` (價格) 三個核心欄位。
- **自動換頁**：預設自動爬取前 5 頁（共 200 筆商品）。
- **輕量依賴**：僅需 `requests` 函式庫，不需要安裝 WebDriver。

## 🛠️ 技術棧
- **語言**: Python 3.x
- **主要套件**: `requests` (API 請求處理)

## 🚀 快速開始

### 1. 安裝必要套件
在使用前，請確保已安裝 `requests`：
```bash
pip install requests
