<script>
	// image source:
	let src = "/src/assets/kitty.png";

	// name is our variable:
	let name = "cat";
</script>

<!-- image given dynamic source attribute, with alt text -->
<img {src} alt="a cat." />

<!-- using curly braces inside attributes, referencing variable in the script block -->
<img {src} alt="a {name}." />

<!-- shorthand attributes: if the name and value of the attribute are the same -->
<img {src} alt="a {name}." />

<style>
	/* big fucking image- don't be taller than 200px */
	img {
		max-height: 200px;
	}
</style>
