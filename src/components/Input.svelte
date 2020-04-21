<script>
  export let value;
</script>

<style>
  main {
    display: flex;
    flex-direction: column;
    border: 2px dotted #ccc;
    background: yellow;
    padding: 10px;
  }
  input {
    border: 2px solid #ccc;
    border-radius: 5px;
  }
  span {
    font-style: oblique;
  }
</style>

<main>
  <input type="text" bind:value />
  <br />
  <span>{value}</span>
</main>
