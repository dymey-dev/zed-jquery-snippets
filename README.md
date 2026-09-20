# Zed jQuery Snippets

A comprehensive collection of 128+ jQuery snippets for the [Zed editor](https://zed.dev/), designed to accelerate JavaScript and DOM development with intelligent autocomplete and placeholder support.

## ✨ Features

- **128+ Production-Ready Snippets**: Complete coverage of jQuery methods, AJAX shortcuts, event handlers, and DOM manipulation.
- **Smart Placeholders**: Tab-navigable parameters (`$1`, `$2`, `$0`) for fast workflow execution.
- **AJAX & Async Utilities**: Shortcuts for `$.ajax`, `$.get`, `$.post`, `$.getJSON`, `$.getScript`, and ASP.NET Web Services.
- **Event Handling & Binding**: Clean patterns for `.on()`, `.off()`, `.click()`, `.hover()`, `.submit()`, `.trigger()`, and delegated events.
- **Effects & Animations**: Built-in triggers for `.fadeIn()`, `.fadeOut()`, `.slideDown()`, `.slideUp()`, `.animate()`, and toggle methods.
- **Plugin Boilerplate**: Quick starter template (`jqPlugin`) for building custom jQuery plugins.

---

## 📦 Installation

### Via Zed Extensions (Recommended)

1. Open **Zed editor**.
2. Press `Cmd + Shift + P` (macOS) or `Ctrl + Shift + P` (Windows/Linux) to open the command palette.
3. Type `extensions` and select `zed: extensions`.
4. Search for **jQuery Snippets**.
5. Click **Install**.

### Manual Installation

1. Clone this repository or copy the directory:
   ```bash
   git clone https://github.com/dymey-dev/zed-jquery-snippets.git
   ```

2. Copy the folder to your Zed extensions directory:
   - **macOS**: `~/.config/zed/extensions/`
   - **Linux**: `~/.config/zed/extensions/`
   - **Windows**: `%APPDATA%\Zed\extensions\`

3. Restart Zed.

---

## 🚀 Quick Start Examples

| Prefix | Description | Generated Code |
|--------|-------------|----------------|
| `jqDocReady` | Document Ready Handler | `$(document).ready(function () { ... });` |
| `jqDocReadyShort` | Short Document Ready | `$(function () { ... });` |
| `jqAjax` | Asynchronous AJAX Request | `$.ajax({ type: "GET", url: "...", ... });` |
| `jqOn` | Event Handler Binding | `$(selector).on('event', function (e) { ... });` |
| `jqClick` | Click Event | `$(selector).click(function (e) { ... });` |
| `jqAppend` | Append Content | `$(selector).append(content);` |
| `jqCssSet` | Set CSS Property | `$(selector).css('property', 'value');` |
| `jqFadeIn` | Fade In Effect | `$(selector).fadeIn('slow');` |
| `jqPlugin` | Custom jQuery Plugin | `(function ($) { $.fn.pluginName = ... })(jQuery);` |

---

## 📚 Snippet Reference

### 1. Document & Initialization
- `jqDocReady` — `$(document).ready(...)` full block.
- `jqDocReadyShort` — `$(function () { ... });` shorthand syntax.
- `func` — Anonymous function callback block.

### 2. AJAX & HTTP Requests
- `jqAjax` — Full `$.ajax` configuration with success callback.
- `jqAjaxAspNetWebService` — `$.ajax` tuned for ASP.NET JSON web services.
- `jqGet` — `$.get()` HTTP GET request helper.
- `jqGetJson` — `$.getJSON()` helper for remote JSON payload fetching.
- `jqGetScript` — `$.getScript()` dynamic script loading helper.
- `jqPost` — `$.post()` HTTP POST request helper.
- `jqLoadGet` / `jqLoadPost` — Load HTML response into DOM element via GET/POST.

### 3. DOM Insertion & Manipulation
- `jqAfter` / `jqBefore` — Insert content after or before target elements.
- `jqAppend` / `jqAppendTo` — Append content inside elements or target.
- `jqPrepend` / `jqPrependTo` — Prepend content inside elements or target.
- `jqInsertAfter` / `jqInsertBefore` — Place elements before/after selector.
- `jqClone` / `jqCloneWithEvents` — Deep clone element nodes with/without event listeners.
- `jqEmpty` / `jqRemove` — Clear inner content or detach nodes from DOM.
- `jqReplaceAll` / `jqReplaceWith` — Replace target elements with new content.
- `jqWrap` / `jqWrapAll` / `jqWrapInner` — Wrap HTML structure around matched nodes.

### 4. Attributes, Properties & Classes
- `jqAttrGet` / `jqAttrSet` / `jqAttrRemove` — Manage element attributes.
- `jqAttrSetObj` — Set multiple attributes using an object literal.
- `jqClassAdd` / `jqClassRemove` — Add or remove CSS classes.
- `jqClassToggle` / `jqClassToggleSwitch` — Toggle class state dynamically.
- `jqHasClass` — Check if element contains a specific class.
- `jqValGet` / `jqValSet` — Read or assign form control values.
- `jqHtmlGet` / `jqHtmlSet` — Read or write inner HTML.
- `jqTextGet` / `jqTextSet` — Read or write text content safely.

### 5. CSS & Styling
- `jqCssGet` — Retrieve CSS property value.
- `jqCssSet` — Set a single CSS property.
- `jqCssSetObj` — Set multiple CSS rules with object map.
- `jqHeightGet` / `jqHeightSet` — Read or modify element height.
- `jqWidthGet` / `jqWidthSet` — Read or modify element width.
- `jqInnerHeight` / `jqInnerWidth` — Dimensions including padding.
- `jqOuterHeight` / `jqOuterWidth` — Dimensions including padding and borders.

### 6. Events & Triggers
- `jqOn` / `jqOne` — Attach persistent or one-time event handlers.
- `jqOff` / `jqUnbind` — Remove event handlers from matched elements.
- `jqClick`, `jqBlur`, `jqChange`, `jqFocus`, `jqSelect`, `jqSubmit`, `jqResize`, `jqScroll` — Core DOM event shortcuts.
- `jqMouseEnter`, `jqMouseLeave`, `jqMouseOver`, `jqMouseOut`, `jqMouseDown`, `jqMouseUp`, `jqMouseMove` — Mouse interaction shortcuts.
- `jqKeyDown`, `jqKeyPress`, `jqKeyUp` — Keyboard event shortcuts.
- `jqHover` — Dual-handler mouseenter/mouseleave helper.
- `jqTrigger` / `jqTriggerHandler` — Trigger events programmatically.

### 7. Effects & Animations
- `jqHide` / `jqShow` / `jqToggle` — Basic visibility toggles.
- `jqFadeIn` / `jqFadeOut` / `jqFadeTo` — Opacity transitions and animations.
- `jqSlideDown` / `jqSlideUp` / `jqSlideToggle` — Vertical slide animations.

---

## 📄 License

This extension is open-source software licensed under the [MIT License](LICENSE).
