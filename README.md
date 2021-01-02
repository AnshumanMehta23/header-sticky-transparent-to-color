# header-sticky-transparent-to-color





function custom_script(){
	echo '<script type="text/javascript" id="yo-script">
			window.onscroll = function() {scrollFunction()};

			function scrollFunction() {
			  if (document.body.scrollTop > 250 || document.documentElement.scrollTop > 250) {
				document.getElementById("yo-header").style.backgroundColor = "#ffffff";
				document.getElementById("yo-header").style.transitionDuration = "1s";
			  } else {
				document.getElementById("yo-header").style.backgroundColor = "rgba(201, 76, 76, 0)";
			  }
			}
	</script>';
}
add_action('wp_head','custom_script');
