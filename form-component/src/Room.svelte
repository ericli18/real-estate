<script>
    import '@picocss/pico'
    import './app.css'
    import Dimensions from './Dimensions.svelte';
    const options = ['bedroom', 'bathroom', 'living room'
    , 'yard', 'garage', 'kitchen'];
    import { onMount } from 'svelte';

    export let form;
    export let index;
  </script>
  
  <main>
   <div>
    <label for="room{index}">We are working on a</label>
    <select id="room{index}" name="room{index}" form={form} required>
      <option value="" disabled selected>Select</option>
      {#each options as option}
        <option>{option}</option>
      {/each}
    </select>
   </div>

   <Dimensions {index} {form}/>

  </main>
  
  <style>
  
  </style>
  