<script>
	import '../app.postcss';
	import Nav from '$lib/Nav.svelte';
</script>

<svelte:head>
	<!-- head content -->
</svelte:head>

<header>
	<Nav />
</header>

<main>
	<slot />
</main>

<footer>
	<div class="content">
		<a href="" class="footer-logo">
			<img src="" alt="" />
		</a>
		<div class="inner-content">
			<ul class="socials" role="list">
				<!-- <li>
					<a href="#">Twitter</a>
				</li>
				<li>
					<a href="#">Github</a>
				</li>
				<li>
					<a href="#">Linkedin</a>
				</li>
				<li>
					<a href="#">Codepen</a>
				</li> -->
				<li>
					<a href="https://twitter.com"
						><svg
							aria-hidden="true"
							focusable="false"
							width="24"
							height="24"
							fill="currentColor"
							class="icon icon-twitter"><use href="#icon-twitter" /></svg
						> Twitter</a
					>
				</li>
				<li>
					<a href="https://facebook.com"
						><svg
							aria-hidden="true"
							focusable="false"
							width="24"
							height="24"
							fill="currentColor"
							class="icon icon-facebook"><use href="#icon-facebook" /></svg
						> Facebook</a
					>
				</li>
				<li>
					<a href="https://linkedin.com"
						><svg
							aria-hidden="true"
							focusable="false"
							width="24"
							height="24"
							fill="currentColor"
							class="icon icon-linkedin"><use href="#icon-linkedin" /></svg
						> LinkedIn</a
					>
				</li>
				<li>
					<a href="https://youtube.com"
						><svg
							aria-hidden="true"
							focusable="false"
							width="24"
							height="24"
							fill="currentColor"
							class="icon icon-youtube"><use href="#icon-youtube" /></svg
						> YouTube</a
					>
				</li>
				<li>
					<a href="https://twitch.tv"
						><svg
							aria-hidden="true"
							focusable="false"
							width="24"
							height="24"
							fill="currentColor"
							class="icon icon-twitch"><use href="#icon-twitch" /></svg
						> Twitch</a
					>
				</li>
			</ul>
			<div class="footer-copy">
				<p>&copy; 2021 Dorian C Brown.</p>
			</div>
		</div>
	</div>
</footer>

<slot />

<style>
</style>
