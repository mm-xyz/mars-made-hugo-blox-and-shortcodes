# Link Preview Card Shortcode

[English](#english) | [中文](#中文)

## English

### Description
A shortcode for creating beautiful link preview cards that display titles, descriptions, and thumbnails from external links.

### Usage

```hugo
{{</* link-preview-card 
    url="https://example.com"
    title="Website Title"
    description="Website Description"
    image="https://example.com/image.jpg"
*/>}}
```

### Parameters

- `url`: Target website URL (required)
- `title`: Preview card title (optional, will attempt to fetch from target website if not provided)
- `description`: Preview card description (optional, will attempt to fetch from target website if not provided)
- `image`: Preview image URL (optional, will attempt to fetch from target website if not provided)

### Features

- Automatic website metadata retrieval
- Responsive design
- Elegant hover effects
- Dark mode support
- Graceful fallback for failed image loading

### Styling

The preview card features modern design elements, including:
- Rounded corners
- Shadow effects
- Responsive images
- Text overflow protection
- Gradient animations

### Alfred Workflow Integration

To make it easier to generate link preview cards, you can use our Alfred Workflow that automatically fetches metadata from web pages:

- GitHub Repository: [get_preview_info](https://github.com/mm-xyz/alfred-scripts/tree/main/get_preview_info)
- Features:
  - Automatically extracts titles, descriptions, and preview images using Open Graph tags
  - Generates Hugo shortcode format
  - Handles SSL certificate warnings
  - Proper error handling

For installation and usage instructions, please visit the workflow repository.

## 中文

### 描述
這個 shortcode 用於創建美觀的鏈接預覽卡片，可以顯示外部鏈接的標題、描述和縮略圖。

### 使用方法

```hugo
{{</* link-preview-card 
    url="https://example.com"
    title="網站標題"
    description="網站描述"
    image="https://example.com/image.jpg"
*/>}}
```

### 參數說明

- `url`: 目標網站的 URL（必填）
- `title`: 預覽卡片標題（可選，如果未提供將嘗試從目標網站獲取）
- `description`: 預覽卡片描述（可選，如果未提供將嘗試從目標網站獲取）
- `image`: 預覽圖片 URL（可選，如果未提供將嘗試從目標網站獲取）

### 特色

- 自動獲取網站元數據
- 響應式設計
- 優雅的懸停效果
- 支援深色模式
- 圖片加載失敗時的優雅降級處理

### 樣式

預覽卡片採用現代化的設計，包括：
- 圓角邊框
- 陰影效果
- 圖片自適應
- 文字溢出保護
- 漸變動畫效果

### Alfred Workflow 整合

為了更方便地生成鏈接預覽卡片，您可以使用我們的 Alfred Workflow，它能自動從網頁獲取元數據：

- GitHub 倉庫：[get_preview_info](https://github.com/mm-xyz/alfred-scripts/tree/main/get_preview_info)
- 功能特點：
  - 使用 Open Graph 標籤自動提取標題、描述和預覽圖片
  - 生成 Hugo shortcode 格式
  - 處理 SSL 證書警告
  - 完善的錯誤處理

安裝和使用說明請訪問 workflow 倉庫。 