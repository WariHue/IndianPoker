<script lang="ts">
  import Card from "./lib/Card.svelte";
  let myNumberOfCard = 1
  const click = (type:string): void => {
    if(myNumberOfCard >= 10)
    {}else
      myNumberOfCard++
  }
</script>

<main>
  <hi class="j">Hello WariHue!</hi>
  <button on:click={() => {click("Heart")}}>a</button>
  <Card num={myNumberOfCard}/>
</main>

<style>
  .j {
    color: blue;
    font-size: 10rem;
  }
</style>