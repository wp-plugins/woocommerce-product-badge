=== WooCommerce Product Badge ===
Contributors: terrytsang
Tags: woocommerce, ecommerce, product, new, sale, featured, badge
Requires at least: 3.8.1
Tested up to: 3.9.1
Stable tag: 1.0.2
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

Displays 'New', 'Sale' and 'Featured' badge on WooCommerce products.

== Description ==

A WooCommerce plugin that let you display 'New', 'Sale' (Save %) and 'Featured' badge at shop and product page.

In WooCommerce Sidebar Menu, there will be a new submenu link called 'Product Badge' where you can:

*   Enabled / Disabled the plugin
*   Display Position (Product Page)
*   Show "New" Badge
*   New Product with How Many Days?
*   Show "Sale" Badge
*   Show "Featured" Badge

= Features =

*   Displays 'New', 'Sale' and 'Featured' badge on WooCommerce products.
*   2 languages available : English UK (en_GB) and Chinese (zh_CN)

= IMPORTANT NOTES =

*   If you need to add new language file, do use POEdit and open 'wc-product-badge.pot' file and save the file as wc-product-badge-[language code].po, then put that into languages folder for this plugin.

= Most Popular Plugins by Terry Tsang =

*   [WooCommerce Custom Checkout Options](http://terrytsang.com/shop/shop/woocommerce-custom-checkout-options/)
*   [WooCommerce Social Buttons PRO](http://terrytsang.com/shop/shop/woocommerce-social-buttons-pro/)
*   [WooCommerce Extra Fee Option PRO](http://terrytsang.com/shop/shop/woocommerce-extra-fee-option-pro/)

== Installation ==

1. Upload `woocommerce-product-badge` to the `/wp-content/plugins/` directory
2. Activate the plugin through the 'Plugins' menu in WordPress
3. You can enable 'New, Sale' and 'Featured' option.
4. Define how 'New' products must be (in days) to receive the 'New' badge on the shop and product page.
5. Done!

== Frequently Asked Questions ==

= I want to style the badge myself, how do I remove the default styles =

There are only a couple of styles applied to the badge. Although not best practise it's probably safe to just overwrite these with your own css. However, if you want to do it properly you can either dequeue the css:

`
add_action( 'wp_enqueue_scripts', 'remove_product_badge_styles', 30 );
function remove_product_badge_styles() {
	wp_dequeue_style( 'wc-product-badge-stylesheet' );
}
`


== Screenshots ==

1. The WooCommerce > Product Badge option page.

2. The shop page with product badges.

3. The product page with Sale and New badge.

4. The mobile layout for product page.

5. The product badge/label shown "After Product Price" as Display Position option.

== Changelog ==

= 1.0.2 =
*   Make product label text "New", "Featured" and "Sale Save (%)" translateable 

= 1.0.1 =
*   Fixed undefined variable bugs
*   Add new option "Display Position (Product Page)" to set priority of badges on woocommerce_single_product_summary

= 1.0.0 =
Initial release.