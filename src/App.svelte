<script>
	import 'carbon-components-svelte/css/g100.css'

	import Header from './components/Header.svelte'
	import Main from './components/Main.svelte'

	import { todoList } from './store'
	todoList.useLocalStorage()
</script>

<svelte:head>
	<title>Todo App</title>
</svelte:head>

<Header bind:todoList={$todoList} />
<Main bind:todoList={$todoList} />
