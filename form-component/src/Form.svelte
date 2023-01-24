<link
  rel="stylesheet"
  href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:opsz,wght,FILL,GRAD@20..48,100..700,0..1,-50..200"
/>

<div class="grid">
  <!-- Markup example 1: input is inside label -->
  <label for="firstname">
    First name
    <input
      type="text"
      id="firstname"
      name="firstname"
      placeholder="First name"
      required
    />
  </label>

  <label for="lastname">
    Last name
    <input
      type="text"
      id="lastname"
      name="lastname"
      placeholder="Last name"
      required
    />
  </label>
</div>

<!-- Markup example 2: input is after label -->
<label for="email">Email address</label>
<input
  type="email"
  id="email"
  name="email"
  placeholder="Email address"
  required
/>

<label for="phone">Phone number</label>
<input type="tel" id="phone" name="phone" placeholder="Phone number" required />
<small>We'll never share your email or phone number with anyone else.</small>

<div class='add-container grid'>
    <div class='container'>
        <span class="material-symbols-outlined">
            add_box
        </span>
        <small>Add a room</small>
    </div>
</div>

<!-- Button -->
<button type="submit">Submit</button>


<style>
    .material-symbols-outlined {
      font-variation-settings:
      'FILL' 0,
      'wght' 300,
      'GRAD' 0,
      'opsz' 48;
      font-size: 50px;
    }

    div.container {
        display: flex;
        flex-direction: column;
        color: hsl(205deg, 10%, 50%);
        align-items: center;
        padding: 1rem;
    }
    
</style>