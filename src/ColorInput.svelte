<script>
    export let colorName, color;
  </script>
  
  <section class="color-range">
    <label for="{colorName}">{colorName}</label>
    <input class="{colorName}" type='range' bind:value={color} max="255"/>
  </section>
  