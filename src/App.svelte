<script>
  // const name= "ashutosh";
  // const role ='<p>Devloper</p>'
  // const  id='heading';
  // const disabled = false
  // const status = 'danger'
  // const success = 'success'
  // const promete = true
  const num = "hdhshdjsh";
</script>

<main>
  <!-- <h1 class="{success}">Hello {name} </h1>
	<h2 class:promete>{@html role}</h2>
	<h1 {id}>this is a heding</h1>
	<button {disabled}>bind</button>
	<h3 class="underline">ashutosh</h3>
	<h2 class="{status}">rama</h2> -->
  {#if num === 0}
    <h1>num is zero</h1>
  {:else if num < 0}
    <h1>numern is negative</h1>
  {:else if num > 0}
    <h1>number is positive</h1>
  {:else}
    <h2>num is not a number</h2>
  {/if}
</main>

<style>
  /* .underline{
		text-decoration: underline;
	}
	.danger{
		color: red;

	}
	.success{
		color: green;
	}
	.promete{
		font-style: italic;
	} */
  main {
    text-align: center;
    padding: 1em;
    max-width: 240px;
    margin: 0 auto;
  }

  h1 {
    color: #ff3e00;
    text-transform: uppercase;
    font-size: 4em;
    font-weight: 100;
  }

  @media (min-width: 640px) {
    main {
      max-width: none;
    }
  }
</style>
