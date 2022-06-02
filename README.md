# SvelteKit demo

This is a small demo of Svelte & SvelteKit for Koodikerho.

## Part 1: Svelte

This part is done as a code-along using the online REPL at https://svelte.dev/repl.

### Showcase the REPL by changing the code

```html
<script>
	let name = 'Koodikerho';
</script>

<h1>Hello {name.toUpperCase()}!</h1>
```

Changing things changes the output.
Template syntax: everything inside `{}` in the template is intepreted as JavaScript.

### Showcase event handling and reactivity

```html
<script>
	let wappuLength = 0;
</script>

<h1>
	Wappu kestää {wappuLength} päivää
</h1>

<button on:click={() => wappuLength++}>
	Lisää yksi päivä
</button>
```

Explain reactivity. The output automatically reacts to state change. 
In React, this would require the use of hooks.

Explain event handler initialization. Show moving it inside the `script`-tag.

## Part 2: SvelteKit
### Prerequisite

Node.js & NPM, fairly recent version

### Initialize the app

```
npm init svelte sveltekit-demo
```
Pick "skeleton project" and answer no to everything for now.

