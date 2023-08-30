<script>
  import ColorVisualiser from "./ColorVisualiser.svelte";
  import ColorInput from "./ColorInput.svelte";
  let red = 0;
  let green = 0;
  let blue = 0;
</script>

<style>
  
</style>

<main>
  <h1>Color Picker 🎨</h1>
  <div class="input">
    <ColorInput colorName="Red" bind:color={red}/>
    <ColorInput colorName="Green" bind:color={red}/>
    <ColorInput colorName="blue" bind:color={red}/>
  </div>

  <ColorVisualiser {red}{green}{blue}/>
</main>
