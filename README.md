# Mars Made Hugo Blox and Shortcodes

這個倉庫包含了一系列自製的 Hugo Shortcodes 和 Blox，可以幫助你更快速地建立美觀的 Hugo 網站。

This repository contains a collection of custom Hugo Shortcodes and Blox to help you build beautiful Hugo websites more efficiently.

## 目錄

[Demo site - Shortcodes](https://anelive.today/hugo-blox-tutorial/mars-made-shortcodes/)


- [customized-callout](#customized-callout) - 可自定義的提示框
- [link-preview-card](#link-preview-card) - 美觀的連結預覽卡片
- [universal-announcement](#universal-announcement) - 通用公告區塊
- [toc-block](#toc-block) - 可摺疊的文章目錄 

## 📦 可用元件 Available Components

### Shortcodes

- `customized-callout`: 可自定義的提示框
  - 支援不同類型(info, warning)
  - 可自定義標題和內容
  - 包含圖示和樣式

- `link-preview-card`: 美觀的連結預覽卡片
  - 支援圖片、標題、描述
  - 顯示網站域名和日期
  - 響應式設計

- `universal-announcement`: 通用公告區塊
  - 顯示最新消息列表
  - 可自定義連結和標題
  - 簡潔的設計風格

- `toc-block`: 可摺疊的文章目錄
  - 自動生成目錄
  - 可摺疊/展開
  - 支援多層級目錄
  - 美觀的樣式和動畫

### Blox

- 待新增...


## 💡 如何使用 How to Use

### Shortcodes 使用方式

1. 找到你想使用的 Shortcode (位於 `shortcodes/` 目錄)
2. 將檔案複製到你的 Hugo 專案的 `layouts/shortcodes/` 目錄中
3. 在你的 Markdown 內容中使用 Shortcode:
   ```markdown
   {{</* shortcode-name */>}}
   ```

### Blox 使用方式

1. 在你的 Hugo 專案的 `config/_default/config.yaml` 中加入:
   ```yaml
   module:
     imports:
       - path: github.com/mm-xyz/mars-made-hugo-blox-and-shortcodes
   ```

2. 在你的頁面中使用 Blox:
   ```markdown
   ---
   type: landing

   sections:
     - block: 'github.mm-xyz.block-name'
       content:
         title: 標題
         text: 內容
   ---
   ```

## 🛠️ 開發指南 Development Guide

### 新增 Shortcode

1. 在 `shortcodes/` 目錄下建立新的 `.html` 檔案
2. 實作 Shortcode 功能
3. 更新本 README 的可用元件清單

### 新增 Blox

1. 在 `blox/` 目錄下建立新的 `.html` 和 `.css` 檔案 (如果需要)
2. 檔案命名格式: `github.mm-xyz.block-name.html`
3. 實作 Blox 功能
4. 更新本 README 的可用元件清單

## 📄 授權 License

本專案採用 MIT 授權條款 - 詳見 [LICENSE.md](LICENSE.md) 檔案。

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.

## 🤝 貢獻 Contributing

歡迎提交 Pull Request 來改善或新增功能！

Pull requests are welcome to improve or add new features!


# [Create Hugo Blox](https://github.com/HugoBlox/create-blox)

**Looking to build and publish a new [Hugo Blox](https://hugoblox.com/blocks/)?**

_[**Hugo Blox**](https://hugoblox.com) makes it easy to create a beautiful website for free, customizing your site without code by using drag-and-drop blocks (aka blox) rendered with Hugo._

## 👉 Core Concepts

- Each blox consists of an HTML file and an optional CSS style file
- Design your blox with [Go Templating](https://gohugo.io/templates/introduction/), [CSS](https://www.w3schools.com/css/), and [Tailwind](https://tailwindcss.com/)
- Unless you are already familiar with Tailwind, it's recommended to use vanilla CSS as Tailwind styles require an extra [compilation step](https://docs.hugoblox.com/reference/extend/#recompile-tailwind) prior to use

## 🧑‍🎨 Create a Block

1. Click the [_Use This Template_](https://github.com/HugoBlox/create-blox/generate) button on GitHub
   1. Name your repository with an appropriate name for your blox collection, such as `johns-hugo-blox`
1. Browse your new GitHub project, click the  `go.mod` file, and then the ✏️ pencil button to edit it
   1. Replace the placeholder URL in `go.mod` with your new GitHub URL in the form `module github.com/<USERNAME>/<COLLECTION-NAME>` where `<USERNAME>` is your GitHub username and `<COLLECTION-NAME>` is a name for your collection of blox
   1. Scroll to the bottom and click _Commit Changes_ to save
1. Browse to the `blox/` folder, click `my-block.html`, and click the ✏️ pencil button to edit it
   1. Rename `my-block.html` in the text box to a unique ID in the form `github.<USERNAME>.<BLOCK-NAME>.html`, again replacing  `<USERNAME>` with your GitHub username and `<BLOCK-NAME>` with your block name. It's important to provide this **globally unique block name**, otherwise another block can conflict with your block.
   1. Repeat the above step to rename the style file, `my-block.css`
   1. Scroll to the bottom and click _Commit Changes_ to save
1. Edit the HTML for your new block
   - Design your blox with [Go Templating](https://gohugo.io/templates/introduction/), [CSS](https://www.w3schools.com/css/), and [Tailwind](https://tailwindcss.com/)
   - You can access page and block (page section) variables using `$page` and `$block`, respectively
   - Check out the [built-in blocks](https://github.com/HugoBlox/hugo-blox-builder/tree/main/modules/blox-tailwind/layouts/partials/blox) for inspiration

### Example

Say your GitHub username is `pikachu` and you wish to create a block named `pokemon`:

1. We click _Use This Template_ and enter `pokemon-hugo-blox` as the project name
1. We replace the first line of `go.mod` with the GitHub repository URL `module github.com/pikachu/hugo-blox-pokemon`
1. We browse to the `blox/` folder, and rename `my-block.html` to `github.pikachu.pokemon.html`
1. We rename `my-block.css` to `github.pikachu.pokemon.css`
1. We customize the HTML in `github.pikachu.pokemon.html` and the style in `github.pikachu.pokemon.css`
1. We add the block to our site and share the block with the community following the guide below

## 🌈 Add the Block to your Site

1. Install the block by referencing it in your `config/_defaults/config.yaml`:
   ```yaml
   module:
     imports:
       # Your block's GitHub URL (replace <USERNAME> and <COLLECTION-NAME> with your GitHub username and block collection name)
       - path: github.com/<USERNAME>/hugo-blox-<COLLECTION-NAME>
   ```
1. Create an instance of your block in a landing page, such as in your homepage at `content/_index.md`:
   ```markdown
   ---
   title: My page
   type: landing

   # Add your page sections below
   # Replace <USERNAME> and <BLOCK-NAME> with your GitHub username and block name, respectively.
   sections:
     - block: 'github.<USERNAME>.<BLOCK-NAME>'
       content:
         title: My title
         text: Add any **markdown** formatted content here - text, images, videos, galleries - and even HTML code!
    ---
   ```

## 📢 Share your block

Add the [hugo-blox](https://github.com/topics/hugo-blox) tag to your block's GitHub repository to help other users find it.

Share your block with the community on [Discord](https://discord.gg/z8wNYzb) and [Twitter](https://twitter.com/intent/tweet?text=I%27m%20creating%20a%20beautiful%20website%20using%20the%20free%20%E2%9D%A4%EF%B8%8F%2C%20open%20source%20Hugo%20Blox%20Website%20Builder%20for%20%40GoHugoIO%20by%20%40GeorgeCushen%20%40GetResearchDev%20%E2%9C%A8%20Have%20some%20feedback%3F%20Please%20comment%20%F0%9F%A4%97&hashtags=MadeWithHugoBlox&url=https://HugoBlox.com/).
