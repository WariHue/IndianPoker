<script lang="ts">
  import Card from "./lib/Card.svelte";
  let myTypeOfCard = "Spade";
  let myNumberOfCard = 1
  const click = (type:string): void => {
    myTypeOfCard= type
    myNumberOfCard++
  }
</script>

<main>
  <hi class="j">{myTypeOfCard}!</hi>
  <button on:click={() => {click("Heart")}}>a</button>
  <Card type={myTypeOfCard} num={myNumberOfCard}/>
</main>

<style>
  .j {
    color: blue;
    font-size: 10rem;
  }
</style>