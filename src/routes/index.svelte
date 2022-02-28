<script>
	import data from '../data.js'

	const { title, subtitle, statement, email } = data

</script>


<svelte:head>
  <title>Iiris Pursiainen - A Finnish artist living in Wales</title>
  <meta name="description" content={statement}>
</svelte:head>

<main class="sassis fill flex column-center-flex-start overflow-auto">

	<div class="flex column maxw70em cmb2 font3 pt2 plr2 ptb8">
		<header class="f4 cmb0-2">
			<h1 class="f4">{title}</h1>
			<h2 class="f4">{subtitle}</h2>
		</header>

		<!-- <aside class="sink">
			<img src="img/sheep.jpg" class="w100pc" />
		</aside> -->

		<article class="font3 f5">
			<blockquote>{statement}</blockquote>
		</article>

		<footer class="f3">
			<a href="mailto:{email}">{email}</a>
		</footer>
	</div>
	
</main>