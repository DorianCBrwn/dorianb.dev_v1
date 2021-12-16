<script>
	import Hamburger from 'svelte-hamburgers';
</script>

<!-- markup (zero or more items) goes here -->
<svelte:head>
	<!-- Import base css -->
	<link
		rel="stylesheet"
		href="https://cdn.jsdelivr.net/npm/svelte-hamburgers@3/dist/css/base.css"
	/>

	<!-- Import spin css (spin is default type) -->
	<link
		rel="stylesheet"
		href="https://cdn.jsdelivr.net/npm/svelte-hamburgers@3/dist/css/types/collapse.css"
	/>
</svelte:head>
<nav id="site-navigation">
	<div class="jump-to-section_container" />
	<a href="/">
		<!-- TODO: replace with svg animated component -->
		<svg xmlns="http://www.w3.org/2000/svg" width="55" height="76" fill="none" viewBox="0 0 55 76">
			<g class="Icon2">
				<path
					stroke="#FEFCFB"
					stroke-width="2"
					d="M28 4c14.36 0 26 11.64 26 26S42.36 56 28 56l-8.5 8V44.5l-8 14.5h-8"
					class="outer-d-path"
				/>
				<path
					fill="#FEFCFB"
					d="M30 46c8.837 0 16-7.163 16-16s-7.163-16-16-16v32z"
					class="inner-d"
				/>
				<circle cx="25" cy="4" r="3.5" stroke="#FEFCFB" class="head-circle" />
				<circle cx="2" cy="59" r="1.5" stroke="#FEFCFB" class="tail-circle" />
				<circle cx="12" cy="65" r="1" fill="#FEFCFB" class="small-circle" />
				<circle cx="27" cy="74" r="2" fill="#FEFCFB" class="large-cirlce" />
				<circle cx="35" cy="62" r="2" fill="#FEFCFB" class="medium-circle" />
			</g>
		</svg>
	</a>
	<div class="primary-nav_container">
		<ul class="primary-nav_links">
			<li><a href="/about">About</a></li>
			<li><a href="/articles">Articles</a></li>
			<li><a href="/work">Work</a></li>
			<li><a href="/contact">Contact</a></li>
		</ul>
		<Hamburger class="hamburger" />
	</div>
</nav>

<style>
	#site-navigation {
		display: flex;
		justify-content: space-around;
		align-items: flex-start;
		background-color: hsl(208, 26%, 40%);
	}

	.primary-nav_container {
		display: flex;
		align-items: center;
		width: 40%;
	}

	.primary-nav_links {
		display: flex;
		justify-content: space-between;
		align-items: center;
	}

	.primary-nav_links a {
		color: rgb(19, 19, 19);
		text-decoration: none;
		font-size: 1.2rem;
		font-weight: bold;
		padding: 0.5rem 1rem;
	}

	.logo {
		align-self: flex-start;
	}

	ul > li {
		text-decoration: none;
	}
</style>
