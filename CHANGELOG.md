# Changelog

## 1.4.0

- Luma / Breeze: on the cart page the bar is now in the summary column, after the order total and before the coupon
  section (it was full width above items and summary). Hyvä is unchanged.

## 1.3.0

- New admin option **Threshold > Exclude Virtual Products** (custom threshold only, default No): virtual products such
  as gift cards are left out of the cart amount, to match shipping methods that ignore virtual items (e.g. Amasty
  Table Rates "Ignore virtual products").

## 1.2.2

- Licence declared in `composer.json` is now `proprietary` (it was MIT), aligned with the other Threecommerce modules. No code changes.

## 1.2.1

- Mini cart (Luma / Breeze): the bar is now the first element of the panel and slim (one line of text, 4 px bar,
  reward steps shown as dots only), instead of a tall box below the subtotal that pushed the products down.
- Fixed the mini cart bar growing to about 150 px in themes whose panel is a wrapping column flex container.

## 1.2.0

- Cart amount chosen in the admin: subtotal after discounts (default) or before cart discounts (coupons and cart
  price rules ignored), each with or without tax.
- Reward steps ("gamification"): extra milestones with amount and name on the bar, markers that turn green when
  reached and a "next reward" message (`{remaining}`, `{threshold}`, `{reward}`). Cart page and mini cart of Luma,
  Breeze and Hyvä.
- Bar and step labels checked on mobile: step sizes follow the width of the bar (container queries).

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
