<script lang="ts">
	import { beforeNavigate, afterNavigate } from '$app/navigation';

	beforeNavigate(({ to, from }) => {
		console.log('beforeNavigate', {
			toX: to?.scroll.x,
			toY: to?.scroll.y,
			fromX: from?.scroll.x,
			fromY: from?.scroll.y
		});
	});

	afterNavigate(({ to, from }) => {
		console.log('afterNavigate', {
			toX: to?.scroll.x,
			toY: to?.scroll.y,
			fromX: from?.scroll.x,
			fromY: from?.scroll.y
		});
	});
</script>

<a href="/">Root</a>
<a href="/two">Two</a>
<a href="/redirect">Redirect</a>
