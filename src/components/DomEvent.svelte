<script>
  let position = { x: 0, y: 0 };
  let active = false;

  function handleMouseMove(event) {
    position.x = event.clientX;
    position.y = event.clientY;
  }

  function handleClick(event) {
    active = true;
  }
</script>

<style>
  div {
    background: #ccc;
    border: 1px solid black;
    width: 100%;
    height: 100%;
    display: flex;
    min-height: 200px;
  }

  .active {
    background: yellow;
  }
</style>

<h1>DOM Events</h1>
<div
  on:mousemove={handleMouseMove}
  on:mousedown={handleClick}
  on:mouseup={() => (active = false)}
  class:active>
  Mouse position (x,y): ({position.x},{position.y});
  <br />
  Active: {active}
</div>
