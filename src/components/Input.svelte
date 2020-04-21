<script>
  export let value;
</script>

<style>
  div {
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

<div>
  <input type="text" bind:value placeholder="Your text here" />
  <br />
  <span>{value}</span>
</div>
