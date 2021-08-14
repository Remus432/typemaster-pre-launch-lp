<script>
  export let bgColor;
  export let color;
  export let hoverBgColor;
</script>

<style>
  button {
    background-color: var(--bg-color);
    border: none;
    border-radius: .8rem;
    color: var(--color);
    cursor: pointer;
    font-weight: bold;
    text-transform: uppercase;
    padding: 2rem;
  }

  button:hover {
    background-color: var(--hover);
    color: #fff;
  }
</style>

<button style="--bg-color: {bgColor}; --color: {color}; --hover: {hoverBgColor}">Pre-order Now</button>