<script>
  import { setContext } from 'svelte'
  import ComponentC from './component/ComponentC.svelte';
import Greet from './component/Greet.svelte'
import Popup from './component/Popup.svelte';
const name ='love sibangi'
const lipu='love khusi'
const obj ={
  name :'mical',
  heroname : 'clark'
}
const userName ='Ashu'

setContext('username-context', userName )
let showPopup = false
function closePopup(event){
  showPopup =false
  console.log(event.detail)
}
</script>

<main>
  <button on:click={() => (showPopup = true)}>show popup</button>
  {#if showPopup}
    <Popup on:close={closePopup}/>
{/if}

 <Greet name='sibangi'  heroname ='Ashutosh'/>
 <Greet name='khusi' heroname ='lipu'/>
 <Greet name='grace' heroname ='ashu'/>
<Greet {name} heroname= {lipu}/>
<Greet {...obj}/>
<h2>App component username - {userName}</h2>
<ComponentC/>
</main>

<style>
 
  
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
