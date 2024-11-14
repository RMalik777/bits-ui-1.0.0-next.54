<script>
	import * as Select from "$lib/components/ui/select/index.js"
	let value = $state("System")
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<Select.Root type="single" bind:value={value}>
  <Select.Trigger>{value}</Select.Trigger>
  <Select.Content>
    <Select.Item value="Light">Light</Select.Item>
    <Select.Item value="Dark">Dark</Select.Item>
    <Select.Item value="System">System</Select.Item>
  </Select.Content>
</Select.Root>
