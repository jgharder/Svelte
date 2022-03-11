<script>
	let user = { loggedIn: false };

	function toggle() {
		user.loggedIn = !user.loggedIn;
	}
</script>

{#if user.loggedIn}
<p>You are drunk!</p>
	<button on:click={toggle}>
		Go home
	</button>
{/if}

{#if !user.loggedIn}
<p>You are boring!</p>
	<button on:click={toggle}>
		Go out
	</button>
{/if}