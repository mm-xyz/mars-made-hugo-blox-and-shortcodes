# Tag Cloud Shortcode

[English](#english) | [中文](#中文)

## English

### Description
A shortcode for creating a tag cloud that dynamically displays article tags or categories, adjusting font sizes based on usage frequency.

### Usage

```hugo
{{</* tag-cloud 
    taxonomy="tags"
    count=20
    font_size_min=1
    font_size_max=2.5
    title="Popular Tags"
    columns=12
*/>}}
```

### Parameters

- `taxonomy`: Category type, defaults to "tags"
- `count`: Number of tags to display, defaults to 20
- `font_size_min`: Minimum font size (rem), defaults to 1
- `font_size_max`: Maximum font size (rem), defaults to 2.5
- `title`: Tag cloud title (optional)
- `columns`: Bootstrap grid columns, defaults to 12

### Features

- Automatic font size adjustment based on tag frequency
- Hover effects: background color change and slight rotation
- Responsive design
- Dark mode support
- Random margins for visual variety

### Styling

The tag cloud uses Bootstrap grid system and custom CSS styles, including:
- Rounded corners
- Gradient backgrounds
- Hover animations
- Adaptive font sizing

## 中文

### 描述
這個 shortcode 用於創建一個標籤雲，可以動態顯示文章標籤或分類，並根據使用頻率調整字體大小。

### 使用方法

```hugo
{{</* tag-cloud 
    taxonomy="tags"
    count=20
    font_size_min=1
    font_size_max=2.5
    title="熱門標籤"
    columns=12
*/>}}
```

### 參數說明

- `taxonomy`: 分類類型，預設為 "tags"
- `count`: 顯示的標籤數量，預設為 20
- `font_size_min`: 最小字體大小（rem），預設為 1
- `font_size_max`: 最大字體大小（rem），預設為 2.5
- `title`: 標籤雲標題（可選）
- `columns`: Bootstrap 網格列數，預設為 12

### 特色

- 根據標籤使用頻率自動調整字體大小
- 懸停效果：背景顏色變化和輕微旋轉
- 響應式設計
- 支援深色模式
- 隨機邊距產生視覺變化

### 樣式

標籤雲使用 Bootstrap 網格系統和自定義 CSS 樣式，包括：
- 圓角設計
- 漸變背景色
- 懸停動畫效果
- 自適應字體大小 