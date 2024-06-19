<script lang="ts">
	import { faEnvelope } from '@fortawesome/free-solid-svg-icons';
	import { faGithub, faXTwitter } from '@fortawesome/free-brands-svg-icons';

	import { FontAwesomeIcon } from '@fortawesome/svelte-fontawesome';
</script>

<footer>
	<ul>
		<li class="email">
			<p>muhyun.kim.dev@gmail.com</p>
			<a href="/contact">
				<FontAwesomeIcon icon={faEnvelope} />
			</a>
		</li>
		<li class="social-contact">
			<p>Follow Me</p>
			<div class="social-contact-link">
				<a href="https://github.com/Muhyun-Kim" target="_blank"
					><FontAwesomeIcon icon={faGithub} /></a
				>
				<a href="https://twitter.com/muhyun_kim" target="_blank"
					><FontAwesomeIcon icon={faXTwitter} /></a
				>
			</div>
		</li>
	</ul>
</footer>

<style>
	ul {
		display: flex;
		width: 100%;
		justify-content: space-between;
	}
	.email {
		display: flex;
		flex-direction: column;
	}
	.email a {
		display: flex;
		justify-content: center;
	}
	.social-contact {
		display: flex;
		flex-direction: column;
	}
	.social-contact-link {
		display: flex;
		justify-content: space-between;
		margin: 0 1rem;
	}
</style>
