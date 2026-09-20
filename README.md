# Zed jQuery Snippets

A comprehensive collection of 128+ jQuery snippets for [Zed editor](https://zed.dev/), designed to accelerate JavaScript and DOM development with intelligent autocomplete, tabstops, and placeholder support.

## ✨ Features

- **128+ Production-Ready Snippets**: Complete coverage of jQuery methods, AJAX shortcuts, event handlers, and DOM manipulation.
- **Smart Placeholders**: Tab-navigable placeholders (`$1`, `$2`, `$0`) for fast workflow execution.
- **Multi-Trigger Document Ready**: Trigger document ready using `jqDocReady`, `ready`, `docready`, `jqready`, `jqDocReadyShort`, or `readyshort`.
- **Wide Language Scope**: Works out of the box in JavaScript (`.js`, `.jsx`), TypeScript (`.ts`), TSX (`.tsx`), HTML (`.html`), and unsaved/Plain Text files.
- **AJAX Utilities**: Complete templates for `$.ajax`, `$.get`, `$.post`, `$.getJSON`, `$.getScript`, and ASP.NET Web Services.
- **Event Handling & Binding**: Shortcuts for `.on()`, `.off()`, `.click()`, `.hover()`, `.submit()`, `.trigger()`, and delegated events.
- **Effects & Animations**: Built-in triggers for `.fadeIn()`, `.fadeOut()`, `.slideDown()`, `.slideUp()`, `.animate()`, and toggle methods.

---

## 📦 Installation

### Via Zed Extensions (Recommended)

1. Open Zed editor
2. Press `Cmd/Ctrl + Shift + P` to open the command palette
3. Type "extensions" and select "zed: extensions"
4. Search for "jQuery Snippets"
5. Click "Install"

### Manual Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/dymey-dev/zed-jquery-snippets
   ```

2. Copy the extension to your Zed extensions directory:
   - **macOS**: `~/.config/zed/extensions/`
   - **Linux**: `~/.config/zed/extensions/`
   - **Windows**: `%APPDATA%\Zed\extensions\`

3. Restart Zed

---

## 🚀 Usage

Simply start typing any jQuery method or prefix shortcut in a `.js`, `.ts`, `.html`, or unsaved buffer. The snippets will automatically appear in the autocomplete menu.

### Quick Start Examples

| Prefix Triggers | Output | Description |
|-----------------|--------|-------------|
| `jqDocReady`, `ready`, `docready`, `jqready` | `$(document).ready(function () { $0 });` | Document ready handler |
| `jqDocReadyShort`, `readyshort`, `jqreadyshort` | `$(function () { $0 });` | Shorthand document ready |
| `jqAjax` | `$.ajax({ type: "$1", url: "$2", ... });` | Async HTTP AJAX request |
| `jqOn` | `$(selector).on('event', function (e) { ... });` | Event handler binding |
| `jqClick` | `$(selector).click(function (e) { ... });` | Click event handler |
| `jqAppend` | `$(selector).append(content);` | Append content |
| `jqCssSet` | `$(selector).css('property', 'value');` | Set CSS property |
| `jqFadeIn` | `$(selector).fadeIn('slow');` | Fade in effect |
| `jqPlugin` | `(function ($) { $.fn.plugin = ... })(jQuery);` | jQuery plugin starter template |

---

## 📋 Available Snippets

### Document & Initialization
- `jqDocReady` / `ready` / `docready` / `jqready` — `$(document).ready(function () { ... });`
- `jqDocReadyShort` / `readyshort` / `jqreadyshort` — `$(function () { ... });` shorthand syntax
- `func` — Anonymous function callback

### AJAX & HTTP Requests
- `jqAjax` — Full `$.ajax` configuration with success callback
- `jqAjaxAspNetWebService` — `$.ajax` tuned for ASP.NET JSON web services
- `jqGet` — `$.get()` HTTP GET request helper
- `jqGetJson` — `$.getJSON()` helper for remote JSON payload fetching
- `jqGetScript` — `$.getScript()` dynamic script loading helper
- `jqPost` — `$.post()` HTTP POST request helper
- `jqLoadGet` / `jqLoadPost` — Load HTML response into DOM element via GET/POST

### DOM Insertion & Manipulation
- `jqAfter` / `jqBefore` — Insert content after or before target elements
- `jqAppend` / `jqAppendTo` — Append content inside elements or target
- `jqPrepend` / `jqPrependTo` — Prepend content inside elements or target
- `jqInsertAfter` / `jqInsertBefore` — Place elements relative to selector
- `jqClone` / `jqCloneWithEvents` — Deep clone element nodes with/without event listeners
- `jqEmpty` / `jqRemove` — Clear inner content or detach nodes from DOM
- `jqReplaceAll` / `jqReplaceWith` — Replace target elements with new content
- `jqWrap` / `jqWrapAll` / `jqWrapInner` — Wrap HTML structure around matched nodes

### Attributes, Properties & Classes
- `jqAttrGet` / `jqAttrSet` / `jqAttrRemove` — Manage element attributes
- `jqAttrSetObj` — Set multiple attributes using an object literal
- `jqClassAdd` / `jqClassRemove` — Add or remove CSS classes
- `jqClassToggle` / `jqClassToggleSwitch` — Toggle class state dynamically
- `jqHasClass` — Check if element contains a specific class
- `jqValGet` / `jqValSet` — Read or assign form control values
- `jqHtmlGet` / `jqHtmlSet` — Read or write inner HTML
- `jqTextGet` / `jqTextSet` — Read or write text content safely

### CSS & Styling
- `jqCssGet` — Retrieve CSS property value
- `jqCssSet` — Set a single CSS property
- `jqCssSetObj` — Set multiple CSS rules with object map
- `jqHeightGet` / `jqHeightSet` — Read or modify element height
- `jqWidthGet` / `jqWidthSet` — Read or modify element width
- `jqInnerHeight` / `jqInnerWidth` — Dimensions including padding
- `jqOuterHeight` / `jqOuterWidth` — Dimensions including padding and borders

### Events & Triggers
- `jqOn` / `jqOne` / `jqOff` — Attach or remove event handlers
- `jqClick`, `jqBlur`, `jqChange`, `jqFocus`, `jqSelect`, `jqSubmit`, `jqResize`, `jqScroll` — Core DOM event shortcuts
- `jqMouseEnter`, `jqMouseLeave`, `jqMouseOver`, `jqMouseOut`, `jqMouseDown`, `jqMouseUp`, `jqMouseMove` — Mouse interaction shortcuts
- `jqKeyDown`, `jqKeyPress`, `jqKeyUp` — Keyboard event shortcuts
- `jqHover` — Dual-handler mouseenter/mouseleave helper
- `jqTrigger` / `jqTriggerHandler` — Trigger events programmatically

### Effects & Animations
- `jqHide` / `jqShow` / `jqToggle` — Basic visibility toggles
- `jqFadeIn` / `jqFadeOut` / `jqFadeTo` — Opacity transitions and animations
- `jqSlideDown` / `jqSlideUp` / `jqSlideToggle` — Vertical slide animations

---

## 🎯 Smart Placeholders

Snippets use tab-navigable placeholders (`$1`, `$2`, etc.) that you can tab through:

```javascript
// Typing 'ready' + Tab
$(document).ready(function () {
  $0
});
```

The `$0` placeholder indicates the final cursor position.

---

## 📄 License

This project is open-source software licensed under the [MIT License](LICENSE).
