<script>
		import Button from "./Button.svelte";
		export let count = 0;
		$: {
		  if (count >= 10) {
		    alert("10 count!!!");
		    count = 0;
		  }
		}
</script>

<style>
  main {
    font-family: sans-serif;
    text-align: center;
  }
</style>

<main>
	<h1>Hello CodeSandbox</h1>
	<h2>Start editing to see some magic happen!</h2>
	<Button bind:count={count} />
</main>