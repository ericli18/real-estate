<script>
  export let index;
  export let form;
</script>

<div class="grid">
  <div>
    <label for="room{index}length">L:</label>
    <input
      type="number"
      id="room{index}length"
      name="room{index}length"
      placeholder="Length"
      {form}
      required
      min="0"
    />
  </div>
  <div>
    <label for="room{index}width">W:</label>
    <input
      type="number"
      id="room{index}width"
      name="room{index}width"
      placeholder="Width"
      {form}
      required
      min="0"
    />
  </div>
  <div>
    <label for="room{index}height">H:</label>
    <input
      type="number"
      id="room{index}height"
      name="room{index}height"
      placeholder="Height"
      required
      {form}
      min="0"
    />
  </div>
</div>

<label for="room{index}notes">Additional notes</label>
<textarea
  id="room{index}notes"
  name="room{index}notes"
  placeholder="Additional notes"
  {form}
/>
