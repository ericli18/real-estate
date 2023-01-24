<script>
    import '@picocss/pico'
    import './app.css'
    const options = ['bedroom', 'bathroom', 'living room'
    , 'yard', 'garage', 'kitchen'];
  </script>
  
  <main>
   <form>
    <select>
      <option value="" disabled selected>Select</option>
      {#each options as option}
        <option>{option}</option>
      {/each}
    </select>
   </form>
  </main>
  
  <style>
  
  </style>
  