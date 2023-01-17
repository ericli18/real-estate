<script>
    function onSubmit(e) {
      const formData = new FormData(e.target);
  
      const data = {};
      for (let field of formData) {
        const [key, value] = field;
        data[key] = value;
      }
      console.log(data)
    }

    function makeRoom(e)
    {
        console.log("Hello");
    }
</script>

<link
  rel="stylesheet"
  href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:opsz,wght,FILL,GRAD@20..48,100..700,0..1,-50..200"
/>
<form on:submit|preventDefault={onSubmit}>
    <div class="grid">
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
    
    <div class='room-wrapper'>
        <button type="button" class='add-container grid' on:click={makeRoom}>
            <div class='container'>
                <span class="material-symbols-outlined">
                    add_box
                </span>
                <small>Add a room</small>
            </div>
        </button>
    </div>
    
    <button type="submit">Submit</button>
</form>


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

    .room-wrapper
    {
        display: flex;
        place-content: center;
    }

    button.add-container {
        all: unset;
        transition: 0.2s ease-in-out;
    }

    button.add-container
    {
        background-color: white;
        border: none;
    }

    button.add-container:active
    {
        background-color:rgb(168, 182, 191);
        border: none;
    }
    
</style>