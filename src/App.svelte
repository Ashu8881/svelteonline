<script>
  // const name= "ashutosh";
  // const role ='<p>Devloper</p>'
  // const  id='heading';
  // const disabled = false
  // const status = 'danger'
  // const success = 'success'
  // const promete = true
  // const num = "hdhshdjsh";
  // const name = ["ram", "sita", "radha"];
  // const fullName = [
  //   { first: "ram", last: "sahu" },
  //   { first: "sita", last: "sahu" },
  //   { first: "radha", last: "patro" },

  // ];
  const  formValues ={
    yearOfExperince :" "
  }
  function submitform(event){
    
   event.preventDefault()
    console.log(formValues)
  }
  
</script>
<main>
  <div><pre>{JSON.stringify(formValues,null,2)}</pre></div>
  <!-- {#each name as names, index}
    <h2>{names} {index + 1}</h2>
  {/each}
  {#each fullName as fullnames, index}
    <h2>{fullnames.first} {fullnames.last} {index + 8}</h2>
  {/each} -->

  <!-- <h1 class="{success}">Hello {name} </h1>
	<h2 class:promete>{@html role}</h2>
	<h1 {id}>this is a heding</h1>
	<button {disabled}>bind</button>
	<h3 class="underline">ashutosh</h3>
	<h2 class="{status}">rama</h2> -->
  <!-- {#if num === 0}
    <h1>num is zero</h1>
  {:else if num < 0}
    <h1>numern is negative</h1>
  {:else if num > 0}
    <h1>number is positive</h1>
  {:else}
    <h2>num is not a number</h2>
    
  {/if} -->
  <form  on:submit={submitform}>
  <div>
    <label for="0-2">0-2</label>
    <input type="radio" id="3-5" value="3-5" bind:group={formValues.yearOfExperince}/>
    <label for="3-5">3-5</label>
    <input type="radio" id="5-7" value="5-7" bind:group={formValues.yearOfExperince}/>
    <label for="5-7">5-7</label>
    <input type="radio" id="7-9" value="7-9" bind:group={formValues.yearOfExperince}/>

  </div>
</form>
  <div>
    <button>Submitt</button>
  </div>
</main>
<style>
input +label{
  display: inline-flex;
}

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
  /* h1 {
    color: #ff3e00;
    text-transform: uppercase;
    font-size: 4em;
    font-weight: 100;
  } */
  @media (min-width: 640px) {
    main {
      max-width: none;
    }
  }
</style>
