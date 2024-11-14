<script>
	import * as Select from "$lib/components/ui/select/index.js"
	let value = $state()
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<Select.Root type="single" value={value}>
  <Select.Trigger>{value}</Select.Trigger>
  <Select.Content>
    <Select.Item value="light">Light</Select.Item>
    <Select.Item value="dark">Dark</Select.Item>
    <Select.Item value="system">System</Select.Item>
  </Select.Content>
</Select.Root>
