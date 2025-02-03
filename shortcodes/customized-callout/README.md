# Customized Callout Shortcode

[English](#english) | [中文](#中文)

## English

### Description
A shortcode for creating custom callout boxes to highlight important information, warnings, or tips.

### Usage

```hugo
{{</* customized-callout 
    type="info"
    title="Tip"
    icon="lightbulb"
*/>}}
This is an important tip message
{{</* /customized-callout */>}}
```

### Parameters

- `type`: Callout type (options: info, warning, danger, success, note), defaults to info
- `title`: Callout title (optional)
- `icon`: Icon name (using Font Awesome icons, optional)

### Features

- Multiple preset styles
- Custom icon support
- Markdown content support
- Responsive design
- Dark mode support

### Styling

The callout box features modern design elements, including:
- Different color schemes for types
- Icon integration
- Rounded corners
- Gradient backgrounds
- Content area formatting

## 中文

### 描述
這個 shortcode 用於創建自定義的提示框，可以用來突出顯示重要信息、警告或提示。

### 使用方法

```hugo
{{</* customized-callout 
    type="info"
    title="提示"
    icon="lightbulb"
*/>}}
這是一個重要的提示信息
{{</* /customized-callout */>}}
```

### 參數說明

- `type`: 提示框類型（可選值：info、warning、danger、success、note），預設為 info
- `title`: 提示框標題（可選）
- `icon`: 圖標名稱（使用 Font Awesome 圖標，可選）

### 特色

- 多種預設樣式
- 支援自定義圖標
- 支援 Markdown 內容
- 響應式設計
- 支援深色模式

### 樣式

提示框採用現代化的設計，包括：
- 不同類型的顏色方案
- 圖標集成
- 圓角邊框
- 漸變背景
- 內容區域格式化 