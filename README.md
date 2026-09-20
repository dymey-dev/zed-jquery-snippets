# Zed jQuery Snippets

A comprehensive collection of jQuery snippets for [Zed editor](https://zed.dev/), designed to accelerate JavaScript and DOM development with intelligent autocomplete and placeholder support.

## ✨ Features

- **128+ Production-Ready Snippets**: Complete coverage of jQuery methods, AJAX shortcuts, event handlers, and DOM manipulation.
- **Smart Placeholders**: Tab-navigable placeholders for efficient coding (`$1`, `$2`, `$0`).
- **DOM & Ready Handlers**: `jqDocReady` and `jqDocReadyShort` for fast document setup.
- **AJAX Utilities**: Complete templates for `$.ajax`, `$.get`, `$.post`, `$.getJSON`, and `$.getScript`.
- **Event Handling & Binding**: Shortcuts for `.on()`, `.off()`, `.click()`, `.hover()`, `.submit()`, and `.trigger()`.
- **Effects & Animations**: Triggers for `.fadeIn()`, `.fadeOut()`, `.slideDown()`, `.slideUp()`, and `.animate()`.

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

## 🚀 Usage

Simply start typing any jQuery method or use prefix shortcuts. The snippets will appear in the autocomplete menu.

### Quick Start Examples

| Prefix | Output | Description |
|--------|--------|-------------|
| `jqDocReady` | `$(document).ready(function () { $0 });` | Document ready handler |
| `jqDocReadyShort` | `$(function () { $0 });` | Shorthand document ready |
| `jqAjax` | `$.ajax({ type: "$1", url: "$2", ... });` | Async HTTP AJAX request |
| `jqOn` | `$(selector).on('event', function (e) { ... });` | Event handler binding |
| `jqClick` | `$(selector).click(function (e) { ... });` | Click event handler |
| `jqAppend` | `$(selector).append(content);` | Append content |
| `jqCssSet` | `$(selector).css('property', 'value');` | Set CSS property |
| `jqFadeIn` | `$(selector).fadeIn('slow');` | Fade in effect |
| `jqPlugin` | `(function ($) { $.fn.plugin = ... })(jQuery);` | jQuery plugin starter |

## 📋 Available Snippets

### Document & Initialization
- `jqDocReady` - `$(document).ready(function () { ... });`
- `jqDocReadyShort` - `$(function () { ... });` shorthand
- `func` - Anonymous function callback

### AJAX & HTTP Requests
- `jqAjax` - Asynchronous AJAX request
- `jqAjaxAspNetWebService` - ASP.NET JSON Web Service request
- `jqGet` - HTTP GET request helper
- `jqGetJson` - Fetch JSON payload
- `jqGetScript` - Load external script
- `jqPost` - HTTP POST request helper
- `jqLoadGet` / `jqLoadPost` - Load HTML response into DOM

### DOM Insertion & Manipulation
- `jqAfter` / `jqBefore` - Insert content after or before target
- `jqAppend` / `jqAppendTo` - Append content to matched elements
- `jqPrepend` / `jqPrependTo` - Prepend content to matched elements
- `jqInsertAfter` / `jqInsertBefore` - Place elements relative to selector
- `jqClone` / `jqCloneWithEvents` - Deep clone elements
- `jqEmpty` / `jqRemove` - Clear content or remove elements from DOM
- `jqReplaceAll` / `jqReplaceWith` - Replace target elements
- `jqWrap` / `jqWrapAll` / `jqWrapInner` - Wrap HTML structure around nodes

### Attributes & CSS
- `jqAttrGet` / `jqAttrSet` / `jqAttrRemove` - Manage attributes
- `jqClassAdd` / `jqClassRemove` / `jqClassToggle` - Manage classes
- `jqHasClass` - Check if element has class
- `jqCssGet` / `jqCssSet` / `jqCssSetObj` - Manage CSS properties
- `jqValGet` / `jqValSet` - Form control values
- `jqHtmlGet` / `jqHtmlSet` - Inner HTML content
- `jqTextGet` / `jqTextSet` - Text content

### Events & Binding
- `jqOn` / `jqOne` / `jqOff` - Bind and unbind events
- `jqClick`, `jqBlur`, `jqChange`, `jqFocus`, `jqSelect`, `jqSubmit`, `jqResize`, `jqScroll` - Core event handlers
- `jqMouseEnter`, `jqMouseLeave`, `jqMouseOver`, `jqMouseOut`, `jqMouseDown`, `jqMouseUp`, `jqMouseMove` - Mouse events
- `jqKeyDown`, `jqKeyPress`, `jqKeyUp` - Key events
- `jqHover` - Hover state handler
- `jqTrigger` / `jqTriggerHandler` - Trigger events programmatically

### Effects & Animations
- `jqHide` / `jqShow` / `jqToggle` - Visibility toggles
- `jqFadeIn` / `jqFadeOut` / `jqFadeTo` - Fade animations
- `jqSlideDown` / `jqSlideUp` / `jqSlideToggle` - Slide animations

## 🎯 Smart Placeholders

Snippets use tab-navigable placeholders (`$1`, `$2`, etc.):

```javascript
// Typing 'jqClick' + Tab
$(selector).click(function (e) {
  $0
});
```

The `$0` placeholder indicates the final cursor position.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
