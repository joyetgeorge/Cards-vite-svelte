<script>
  import Card from './lib/Card.svelte'

  let data = [
    {
      icon: 'https://img.icons8.com/external-tanah-basah-basic-outline-tanah-basah/48/0471FF/external-clipboard-accounting-tanah-basah-basic-outline-tanah-basah.png',
      label: 'Project management',
      description: 'Create tasks, track time, and update progress all in one place'
    },
    {
      icon: 'https://img.icons8.com/fluency-systems-regular/48/CF00FF/clock--v3.png',
      label: 'Time tracking',
      description: 'Discover how much time your team is spending on their work.'
    },
    {
      icon: 'https://img.icons8.com/material-rounded/48/FF7600/tear-off-calendar.png',
      label: 'Resource planning',
      description: 'Monitor how your resources are utilized across projects.'
    },
    {
      icon: 'https://img.icons8.com/fluency-systems-regular/48/02B94C/us-dollar-circled--v1.png',
      label: 'invoicing',
      description: 'Save time by invoicing based on reported time for accurate billing.'
    }
  ]
</script>

<main>
  <div class="cards">
    {#each data as item, index}
       <Card item={item} index={index}/>
    {/each}
  </div>
</main>

<style>
  .cards {
    height: 100vh;
    display: flex;
    justify-content: space-evenly;
    gap: 2rem;
    align-items: center;
  }
</style>