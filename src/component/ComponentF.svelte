<script>
  import { getContext } from "svelte";
const userName= getContext ('username-context')
</script>
<h2>Child F Component</h2>
<h2>Child f userName-{userName} </h2>