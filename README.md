# WKWebView Demo – Overview

This project demonstrates how to integrate and extend `WKWebView` in an iOS app.  
A **full-featured `WKWebView` app** with navigation, JavaScript communication (both directions), and delegate handling for web page interactions

## 📌 Key Implementations
- **WKWebView Setup**  
  - Configured with `WKWebViewConfiguration`  
  - Loaded a local `demo.html` file  

- **Navigation Controls**  
  - Added **Back**, **Forward**, and **Refresh** buttons in the navigation bar  
  - Updated button states dynamically using `canGoBack` / `canGoForward`  

- **Delegates**  
  - Implemented **`WKNavigationDelegate`** for page load lifecycle, error handling, and navigation policies  
  - Implemented **`WKUIDelegate`** for handling JavaScript alerts, confirms, prompts, `window.open`, and `window.close`  

- **JavaScript Bridge (JSB)**  
  - **Web → Swift** via `WKScriptMessageHandler` (`iosListener`, `navigateAppleWebsite`)  
  - **Swift → Web** via `evaluateJavaScript` (example: change background color after load)
  
---
