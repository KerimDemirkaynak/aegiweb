# Aegisub Modern Download Page

Aegisub is one of the most popular open-source tools for creating professional-quality subtitles. This project is a **modern, fast, and completely single-file** web page designed to provide users with the latest version of Aegisub (the TypesettingTools fork) and popular plugins (e.g., Turkish Dictionary).

## ✨ Features

* **📦 Single-File Architecture:** All HTML, CSS, and JavaScript codes are contained within a single `index.html` file. It does not require any extra stylesheets or external dependencies.
* **🌍 Automatic Language Detection (i18n):** Automatically detects the visitor's browser language and presents the site in that language. It currently supports **English, Turkish, Spanish, Russian, and Chinese**.
* **💻 Smart OS Detection:** Detects whether the visitor is using Windows, macOS, or Linux and automatically adapts the text of the main download button at the top (e.g., *"Download for Windows"*).
* **🔗 Up-to-Date Redirects:** Instead of old, abandoned Aegisub versions, it redirects to the latest release of the actively community-developed [TypesettingTools/Aegisub](https://github.com/TypesettingTools/Aegisub) repository.
* **🇹🇷 Turkish Dictionary Integration:** Includes a direct download link for the [automatic Turkish spell checker plugin](https://github.com/kerimdemirkaynak/aegisub-turkish-dictionary) for Aegisub.
* **📱 Fully Responsive Design:** Built on a premium dark theme (Dark Mode) and looks flawless on all screens, including mobile, tablet, and desktop.

## 🚀 Installation and Usage

You do not need a server or database setup for the site to work. It is simply a static HTML file.

1. Clone this repository or download it as a `.zip`.
2. Open the `index.html` file in any web browser.
3. If you want to publish it, you can host this repository for free in seconds via **GitHub Pages**, **Vercel**, **Netlify**, or **Cloudflare Pages**.

## 🛠️ Development (Adding a New Language)

Adding a new language to the page is very easy. Simply open the `index.html` file with a text editor and add your new language code into the `const i18n = { ... }` object located in the `<script>` section at the bottom.

Example (to add German):
```javascript
de: {
    meta_title: "Aegisub | Erweiterter Untertitel-Editor",
    meta_desc: "Aegisub ist ein kostenloses Open-Source-Tool...",
    nav_feat: "Eigenschaften", 
    nav_dl: "Herunterladen",
    // ...other translations
}
```
Then, do not forget to add the `<option value="de">Deutsch</option>` line to the `<select id="langSwitcher">` menu inside the `<nav>`.

## 📄 License
The source code of this project is open-source, and you can edit and use it as you wish. Aegisub's own source codes are subject to the BSD and ISC licenses. The logo and logotype used in the design belong to the original Aegisub project.
