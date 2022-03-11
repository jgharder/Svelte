<script>
	let count = 1;

	// the `$:` means 're-run whenever these values change'
	$: doubled = count * 4;
	$: quadrupled = doubled * 8;

	function handleClick() {
		count += 1;
	}
</script>

<button on:click={handleClick}>
	Count: {count}
</button>

<p>{count} * 4 = {doubled}</p>
<p>{doubled} * 8 = {quadrupled}</p>