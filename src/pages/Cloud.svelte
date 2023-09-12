<script lang="ts">
	import InnerPages from '../components/InnerPages.svelte';
	import Box from '../components/cloud/Box.svelte';
	import Grid from '../components/cloud/Grid.svelte';
</script>

<InnerPages image="cloud" title="Cloud - Data Center & Cyber Security">
  <Grid title="Data Center">  
    <Box title="Operation">
      Attività relative all'operatività e alla gestione tecnico-sistemistica del Data Center.
    </Box>

    <Box title="Transformation">
      Attività relative all'innovazione e trasformazione dei Data Center da modelli tradizionali ad 
      approcci legati alla virtualizzazione, al Cloud e/o al "software defined".
    </Box>

    <Box title="Creation">
      Predisposizione di Data Center e infrastrutture a supporto di applicazioni e servizi.
    </Box>

    <Box title="Support">
      Introduzione ai nuovi servizi Cloud e migrazione delle infrastrutture, piattaforme e servizi tradizionali verso il modello Cloud garantendo livelli di servizio Enterprise uniti alle caratteristiche avanzate abilitate dalla modalità "as-a-Service" di tipo IaaS, PaaS e BaaS.
    </Box>
  </Grid>

  <Grid title="Software Projects">
    <Box title="Digital Transformation">
      Attività relative alla trasformazione di applicazioni sia monolitiche sia multitier gestite "On Premise" o in Hybrid Cloud verso un modello Cloud fully managed o in modalità hybrid secondo necessità.
    </Box>

    <Box title="Containerization">
      Attività relative alla trasformazione e creazione di soluzioni conteinerizzate sia a livello di Sistema Operativo sia di applicazione.
    </Box>

    <Box title="Creation">
      Predisposizione di nuove architetture Cloud sia dal punto di vista ingegneristico sia dal punto di vista applicativo.
    </Box>

    <Box title="Support">
      Introduzione ai nuovi servizi Cloud e migrazione delle infrastrutture, piattaforme e servizi tradizionali verso il modello Cloud garantendo livelli di servizio Enterprise uniti alle caratteristiche avanzate abilitate dalla modalità "as-a-Service" di tipo IaaS, PaaS e BaaS.
    </Box>
  </Grid>
</InnerPages>