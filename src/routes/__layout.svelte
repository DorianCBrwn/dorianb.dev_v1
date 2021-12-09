<script>
</script>

<svelte:head>
	<!-- head content -->
</svelte:head>

<header>
	<nav id="site-navigation">
		<div class="jump-to-section_container" />
		<div class="primary-nav_container">
			<ul class="primary-nav_links">
				//TODO: Fix a tags
				<li><a href="/about" />About</li>
				<li><a href="/articles" />Articles</li>
				<li><a href="/work" />Work</li>
				<li><a href="/contact" />Contact</li>
			</ul>
			//TODO: replace button with hamburger component
			<button />
		</div>
	</nav>
</header>
<main>
	<slot />
</main>
<footer />

<style>
	#site-navigation {
		display: flex;
	}
</style>
