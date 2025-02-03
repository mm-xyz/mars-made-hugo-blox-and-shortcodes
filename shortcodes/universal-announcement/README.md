# Universal Announcement Shortcode

[English](#english) | [中文](#中文)

## English

### Description
A shortcode for displaying global announcements or notification messages with support for multiple styles and customization options.

### Usage

```hugo
{{</* universal-announcement 
    type="info"
    title="Important Announcement"
    content="This is an important announcement message"
    dismissible=true
*/>}}
```

### Parameters

- `type`: Announcement type (options: info, warning, danger, success), defaults to info
- `title`: Announcement title (optional)
- `content`: Announcement content (required)
- `dismissible`: Whether the announcement can be dismissed (true/false), defaults to false

### Features

- Multiple preset styles
- Dismissible functionality
- Responsive design
- Markdown content support
- Dark mode support

### Styling

The announcement banner features modern design elements, including:
- Different color schemes for types
- Rounded corners
- Gradient backgrounds
- Dismiss button animations
- Smooth transitions

## 中文

### 描述
這個 shortcode 用於在網站中顯示全局公告或提示信息，支援多種樣式和自定義選項。

### 使用方法

```hugo
{{</* universal-announcement 
    type="info"
    title="重要公告"
    content="這是一條重要的公告信息"
    dismissible=true
*/>}}
```

### 參數說明

- `type`: 公告類型（可選值：info、warning、danger、success），預設為 info
- `title`: 公告標題（可選）
- `content`: 公告內容（必填）
- `dismissible`: 是否可關閉（true/false），預設為 false

### 特色

- 多種預設樣式
- 可關閉功能
- 響應式設計
- 支援 Markdown 內容
- 支援深色模式

### 樣式

公告橫幅採用現代化的設計，包括：
- 不同類型的顏色方案
- 圓角設計
- 漸變背景
- 關閉按鈕動畫
- 平滑過渡效果 