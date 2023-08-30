<script>
  import ColorVisualiser from "./ColorVisualiser.svelte";
  import ColorInput from "./ColorInput.svelte";
  let red = 0;
  let green = 0;
  let blue = 0;
  $: hexColor = `#${hex(red)}${hex(green)}${hex(blue)}`;
  function hex(color) {
    return color.toString(16).padStart(2, '0');
  }
</script>

<style>
  
</style>

<main>
  <h1>Color Picker 🎨</h1>
  <div class="input">
    <ColorInput colorName="Red" bind:color={red}/>
    <ColorInput colorName="Green" bind:color={green}/>
    <ColorInput colorName="Blue" bind:color={blue}/>
  </div>

  <ColorVisualiser {red}{green}{blue}{hexColor}/>
</main>
