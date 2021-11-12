<script lang="ts">
	let svelte: string
	let typescript: string
	let sass: string

	svelte = 'Svelte'
	typescript = 'Typescript'
	sass = 'Sass'

</script>

<div class="home">
  <h3>Home Page</h3>
  <h3 class="home__svelte">Hello {svelte}</h3>
  <h3 class="home__typescript">Hello {typescript}</h3>
  <h3 class="home__sass">Hello {sass}</h3>
</div>

<style lang="scss">
	$svelte-color: #ff3e00;
	$typescript-color: #3178c6;
	$sass-color: #cf649a;

	.home {
		&__svelte {
			color: $svelte-color;
		}

		&__typescript {
			color: $typescript-color;
		}

		&__sass {
			color: $sass-color;
		}
	}
</style>