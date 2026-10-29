# Changelog

## 1.1.0

- Luma-based themes and Breeze: bar on the cart page (above items and summary) and in the mini cart
  (Knockout component below the subtotal, registered for Breeze in `breeze_default.xml`).
- The cart page template no longer depends on Hyvä (view model passed as layout argument, inline icons).
- "Show in Mini Cart" applies to every theme (section data hidden when off).
- `hyva-themes/magento2-theme-module` is no longer required (suggested).

## 1.0.0

- Free shipping progress bar on the cart page (server rendered) and in the Hyvä cart drawer (customer section data).
- Cart amount = discounted subtotal (coupons and cart price rules included), with or without tax.
- Threshold: custom with per-country overrides, or read from the Free Shipping method.
- Free shipping granted by a cart rule shown as reached.
- Editable messages per store view with `{remaining}` / `{threshold}` placeholders; colors from the admin.
