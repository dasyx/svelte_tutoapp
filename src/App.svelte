<script>
// @ts-nocheck

  import Products from "./components/Products.svelte";
  import Users from "./components/Users.svelte";
  import { Button} from 'sveltestrap';
  import Rating  from './components/Rating.svelte';

  let isValid = true;
  /* import Button from "./components/Button.svelte"; */
</script>

<main>
  <Products />
  <Users />
  <section>
    <!-- <Button text="Click me" color="red" />
    <Button text="Disabled" disabled /> -->
      <Button color="primary">Click Me</Button>
      <Button color="danger" disabled={!isValid} >Click Me</Button>
      <Rating rating= 5 />
  </section>
</main>

<style>
</style>
