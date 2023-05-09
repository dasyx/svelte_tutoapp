<script>
  import { Icon } from "sveltestrap";

  export let rating = 0;
</script>

<h1>Rating : {rating}</h1>

<!-- with an array -->

<!-- {#each Array(5) as _, i}
  {#if rating >= i + 1}
    <Icon name="star-fill" />
  {:else}
    <Icon name="star" />
  {/if}
{/each} -->


<!--Ici, nous utilisons la directive each de Svelte pour boucler sur un tableau vide de longueur 5 (Array(5)), en utilisant la variable _ pour ignorer la valeur de chaque élément et la variable i pour représenter l'index de chaque élément dans la boucle.

À chaque itération de la boucle, nous comparons la note rating avec l'index de l'élément plus un, car les index commencent à zéro. Si la note est supérieure ou égale à l'index plus un, nous affichons une étoile pleine (<Icon name="star-fill" />), sinon nous affichons une étoile vide (<Icon name="star" />).

En résumé, cette instruction utilise la directive each pour boucler sur un tableau vide de longueur 5 et affiche une étoile pleine ou vide pour chaque note en fonction de sa position dans la boucle.-->

{#if rating >= 1}
  <Icon name="star-fill" />
{:else}
  <Icon name="star" />
{/if}

{#if rating >= 2}
  <Icon name="star-fill" />
{:else}
  <Icon name="star" />
{/if}

{#if rating >= 3}
  <Icon name="star-fill" />
{:else}
  <Icon name="star" />
{/if}

{#if rating >= 4}
  <Icon name="star-fill" />
{:else}
  <Icon name="star" />
{/if}

{#if rating >= 5}
  <Icon name="star-fill" />
{:else}
  <Icon name="star" />
{/if}

