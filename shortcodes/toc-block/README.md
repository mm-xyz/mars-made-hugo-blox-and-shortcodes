# TOC Block Shortcode

[English](#english) | [中文](#中文)

## English

### Description
A shortcode for creating a beautiful table of contents block that displays the heading structure of the current page.

### Usage

```hugo
{{</* toc-block 
    title="Table of Contents"
    min_level=2
    max_level=4
    collapsible=true
*/>}}
```

### Parameters

- `title`: TOC block title (optional)
- `min_level`: Minimum heading level (optional, defaults to 2)
- `max_level`: Maximum heading level (optional, defaults to 4)
- `collapsible`: Whether the TOC is collapsible (true/false, defaults to true)

### Features

- Automatic TOC generation
- Smooth scroll to target
- Active position highlighting
- Collapsible/expandable functionality
- Dark mode support

### Styling

The TOC block features modern design elements, including:
- Level indentation
- Hover highlight effects
- Current position indicator
- Collapse/expand animations
- Responsive layout

## 中文

### 描述
這個 shortcode 用於創建一個美觀的目錄區塊，可以顯示當前頁面的標題結構。

### 使用方法

```hugo
{{</* toc-block 
    title="目錄"
    min_level=2
    max_level=4
    collapsible=true
*/>}}
```

### 參數說明

- `title`: 目錄區塊標題（可選）
- `min_level`: 最小標題層級（可選，預設為 2）
- `max_level`: 最大標題層級（可選，預設為 4）
- `collapsible`: 是否可折疊（true/false，預設為 true）

### 特色

- 自動生成目錄結構
- 平滑滾動到目標位置
- 當前閱讀位置高亮
- 可折疊/展開功能
- 支援深色模式

### 樣式

目錄區塊採用現代化的設計，包括：
- 層級縮進
- 懸停高亮效果
- 當前位置指示器
- 折疊/展開動畫
- 響應式佈局 