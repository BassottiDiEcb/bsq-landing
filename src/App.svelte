<script lang="ts">
	import { Router, Route } from "svelte-routing";
	import Home from './pages/Home.svelte'
	import Cloud from './pages/Cloud.svelte'
	import Droni from './pages/Droni.svelte'
	import Laser from './pages/Laser.svelte'
	import Energia from './pages/Energia.svelte'
	import Telecomunicazioni from './pages/Telecomunicazioni.svelte'
	import Virtuale from './pages/Virtuale.svelte'

	export let url = ""
</script>

<Router {url}>
  <div>
    <Route path="/" component={Home} />
    <Route path="/cloud" component={Cloud} />
    <Route path="/droni" component={Droni} />
    <Route path="/laser" component={Laser} />
    <Route path="/energia" component={Energia} />
    <Route path="/telecomunicazioni" component={Telecomunicazioni} />
    <Route path="/virtuale" component={Virtuale} />
  </div>
</Router>