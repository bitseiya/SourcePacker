# SourcePacker

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![.NET Version](https://img.shields.io/badge/.NET-8.0-blueviolet.svg)](https://dotnet.microsoft.com/en-us/download/dotnet/8.0)
[![Platform](https://img.shields.io/badge/Platform-Windows-blue.svg)](https://www.microsoft.com/windows)

**Languages:** **English** | [简体中文](./README.zh-CN.md)

An intuitive GUI tool for developers to easily package an entire codebase into a single XML file. Streamline the process of feeding your project's context to AI models like GPT, Claude, and Gemini with powerful filtering and a simple drag-and-drop interface.

---

## 🌟 Why SourcePacker?

When interacting with Large Language Models (LLMs), you often need to provide a large amount of code as context. Manually copying and pasting multiple files is not only inefficient but also prone to errors, such as missing key files or breaking the code's structure. SourcePacker is designed to solve this problem by allowing you to:

*   **Effortless Consolidation**: Combine complex project structures into a single file, ready for copy-pasting.
*   **Precise Context**: Use smart filters to provide only the core source code to the AI, reducing noise, saving tokens, and improving response quality.
*   **Code Archiving**: Create a single, self-contained file of your source code for easy archiving and sharing.

## 📸 Application Screenshot

<img width="887" height="742" alt="source-packer" src="https://github.com/user-attachments/assets/693d21be-275d-4613-ad3a-7e002df1c89c" />


## ✨ Features

Based on the source code, SourcePacker includes the following key features:

*   **📁 Drag & Drop Support**: Intuitively drag and drop files and folders directly into the application window.
*   **🌳 Smart Filtering**:
    *   **Include by Extension**: Process only the file types you specify (e.g., `.cs`, `.js`, `.py`).
    *   **Exclude by Filename**: Automatically ignore files containing specific keywords (e.g., `-min.`, `.min.`).
    *   **Exclude by Directory**: Automatically skip designated directories (e.g., `bin`, `obj`, `node_modules`).
*   **⚙️ Customizable Configuration**: All filter rules can be easily added or removed from the UI. Your settings are automatically saved for future use.
*   **🖥️ Clean UI**: A modern user interface built with WPF, providing a clear view of your file list and settings.
*   **🌐 Multi-language Support**: Built-in support for English (en-US), Simplified Chinese (zh-CN), and Japanese (ja-JP), with an easy-to-use language switcher.
*   **📦 Single XML Output**: Wraps all file content in `CDATA` blocks to generate a well-formed XML, preventing parsing errors from special characters.


## 🚀How to Use

1.  **Set Output Path**: Click the Browse button to select where you want to save the final XML file.
2.  **Adjust Filters **: In the configuration panel on the right, modify the included extensions or exclusion rules to fit your needs.
3.  **Add Files/Folders**: Drag your project files or the root folder into the list area on the left.
4.  **Export**: Click the "Export to XML" button, and you're done!


## 💻 Technology Stack

*   **Framework**: .NET 8
*   **UI**: WPF (Windows Presentation Foundation)
*   **Serialization**: Newtonsoft.Json (for saving and loading application settings)

## 🙌 Contributing

Contributions are welcome! If you have ideas, find a bug, or want to add a new feature, please feel free to:

*   Open an [Issue](https://github.com/bitseiya/SourcePacker/issues) to discuss it.
*   Create a [Pull Request](https://github.com/bitseiya/SourcePacker/pulls) with your changes.

## 📄 License

This project is licensed under the [MIT License](https://opensource.org/licenses/MIT).
