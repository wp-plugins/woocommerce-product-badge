=== WooCommerce Product Badge ===
Contributors: terrytsang
Tags: woocommerce, ecommerce, product, new, sale, featured, badge
Requires at least: 3.8.1
Tested up to: 3.9.1
Stable tag: 1.0.0
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

Displays 'New', 'Sale' and 'Featured' badge on WooCommerce products.

== Description ==

A WooCommerce plugin that let you display 'New', 'Sale' (Save %) and 'Featured' badge at shop and product page.

== Installation ==

1. Upload `woocommerce-product-badges` to the `/wp-content/plugins/` directory
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

== Changelog ==

= 1.0.0 =
Initial release.