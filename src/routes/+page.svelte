<script>
	import { Alert, Button, Input, Label } from 'flowbite-svelte';

	function clickMe(params) {
		console.log('clicked me');
	}

	function onsubmit(params) {
		alert('submitting');
	}
</script>

<div class="container mx-auto p-4">
	<form method="post" on:submit={onsubmit}>
		<Label>
			<Input type="text" name="name" />
		</Label>
		<Button type='submit'>click me</Button>
	</form>
</div>
