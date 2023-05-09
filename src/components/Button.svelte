<!-- Button.svelte -->
<!-- Button without Sveltestrap -->

<script>
    export let text;
    export let color = 'blue';
    export let disabled = false;
    
    function handleClick() {
      if (disabled) return;
      alert('Button clicked!');
    }
  </script>
  
  <button
    on:click={handleClick}
    class={`button ${color} ${disabled ? 'disabled' : ''}`}
  >
    {text}
  </button>
  
  <style>
    .button {
      border: none;
      border-radius: 4px;
      padding: 8px 12px;
      font-size: 16px;
      cursor: pointer;
    }
  
    .blue {
      background-color: blue;
      color: white;
    }
  
    .red {
      background-color: red;
      color: white;
    }
  
    .disabled {
      opacity: 0.5;
      cursor: not-allowed;
    }
  </style>
  