<script lang="ts">
	const version = __APP_VERSION__;
</script>

<footer class="app-footer">
	<p class="footer-content">
		<span>Created by Rohit Totlani</span>
		<span class="heart">♥</span>
	</p>
	<p class="footer-links">
		<a href="https://github.com/rohit317/askey" target="_blank" rel="noopener noreferrer"
			>Source Code</a
		>
		/
		<a href="https://github.com/rohit317/askey#readme" target="_blank" rel="noopener noreferrer"
			>Project Notes</a
		>
	</p>
	<p class="footer-copyright footer-links">
		© Rohit Totlani, {new Date().getFullYear()}.
		<a href="https://choosealicense.com/licenses/mit/" target="_blank" rel="noopener noreferrer"
			>Licensed under MIT.</a
		>
	</p>
</footer>

<style>
	.app-footer {
		width: 100vw;
		margin-left: -1.5rem;
		margin-bottom: -1.5rem;
		margin-top: 2rem;
		padding: 2rem 1.5rem;
		text-align: center;
		border-top: 1px solid var(--border-color, #333);
		background: var(--bg-secondary, #1a1a1a);
		position: relative;
	}

	.footer-content {
		margin: 0 0 0.5rem 0;
		font-size: 0.95rem;
	}

	.footer-content a {
		color: var(--text-primary, #fff);
		text-decoration: none;
		font-weight: 500;
	}

	.footer-content a:hover {
		text-decoration: underline;
	}

	.heart {
		margin-left: 0.25rem;
		display: inline-block;
		animation: pulse 1.5s ease-in-out infinite;
	}

	@keyframes pulse {
		0%,
		100% {
			transform: scale(1);
		}
		50% {
			transform: scale(1.1);
		}
	}

	.footer-links {
		margin: 0.5rem 0;
		font-size: 0.9rem;
	}

	.footer-links a {
		color: var(--accent-color, #4a9eff);
		text-decoration: none;
	}

	.footer-links a:hover {
		text-decoration: underline;
	}

	.footer-copyright {
		margin: 0.5rem 0 0 0;
		font-size: 0.85rem;
		color: var(--text-secondary, #888);
	}

	.footer-version {
		position: absolute;
		right: 1.5rem;
		bottom: 2rem;
		margin: 0;
	}

	@media (max-width: 815px) {
		.footer-version {
			display: none;
		}
	}

	.version-badge {
		display: inline-flex;
		align-items: center;
		gap: 0.5rem;
		margin-left: 1.15rem;
		padding: 0.4rem 0.8rem;
		background: transparent;
		border: 1px solid var(--border-color, #333);
		color: var(--text-primary, #fff);
		text-decoration: none;
		font-family: 'Inconsolata', monospace;
		font-size: 0.8rem;
		transition:
			background 0.2s ease,
			border-color 0.2s ease;
	}

	.version-badge:hover {
		background: var(--bg-tertiary, #222);
		border-color: var(--gray-500, #666);
		text-decoration: none;
	}

	.fork-icon {
		font-size: 1.2em;
		line-height: 1;
	}
</style>
