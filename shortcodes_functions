function landingpage_header( $atts ) {
	ob_start();
	?>
	<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
	<html xmlns="http://www.w3.org/1999/xhtml" lang="en-US">
	<head profile="http://gmpg.org/xfn/11">
		<meta http-equiv="Content-Type" content="text/html; charset=UTF-8" />
		<title><?php bloginfo('name'); ?><?php wp_title('|', true, 'left'); ?></title>
		<?php wp_head(); ?>
	</head>
	<body <?php body_class(); ?>>
	<?php 
	$content = ob_get_contents();
	ob_clean();
	return $content;
}
add_shortcode( 'landingpage_header','landingpage_header' );

function landingpage_footer( $atts ) {
	ob_start();
	?>
	<?php wp_footer(); ?>
	</body>
	</html>
	<?php
	$content = ob_get_contents();
	ob_clean();
	return $content;
}
add_shortcode( 'landingpage_footer','landingpage_footer' );
