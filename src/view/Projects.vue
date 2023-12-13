<script setup>
  import BodyComponent from "../components/BodyComponent.vue";
</script>

<template>
  <BodyComponent>

    <h1>Progetti multimediali</h1>
    <div></div>
    <p class="p-8">è un'installazione interattiva che consente agli utenti di dipingere virtualmente nello spazio utilizzando il loro corpo come pennello. Utilizzando OpenFrameworks e un sensore Kinect, l'installazione cattura i movimenti del corpo dell'utente e li traduce in tratti e colori su uno schermo virtuale.</p>
    <h3>Tecnologie Utilizzate:</h3>
    <ol class="list-disc list-inside p-5"><li><strong>OpenFrameworks:</strong> Una libreria C++ per la creazione di applicazioni creative e interattive.</li><li><strong>Kinect Sensor:</strong> Per rilevare i movimenti e la posizione del corpo dell'utente.</li><li><strong>Grafica 3D:</strong> Per creare uno spazio virtuale in cui gli utenti possono disegnare.</li><li><strong>Suono:</strong> Per aggiungere un elemento audio all'installazione.</li></ol>
    <h3>Funzionalità Principali:</h3>
    <ol class="list-disc list-inside p-5"><li><p><strong>Rilevamento del Corpo:</strong> Utilizzando il sensore Kinect, il sistema rileva la presenza e i movimenti del corpo dell'utente nello spazio.</p></li><li><p><strong>Trasformazione dei Movimenti in Tratti:</strong> I movimenti del corpo vengono tradotti in tratti sulla "tela" virtuale, consentendo agli utenti di disegnare nello spazio.</p></li><li><p><strong>Colorazione Interattiva:</strong> Gli utenti possono selezionare i colori e applicarli al loro disegno utilizzando gesti specifici riconosciuti dal sensore.</p></li><li><p><strong>Grafica 3D Immersiva:</strong> Il disegno appare in uno spazio 3D, creando un'esperienza immersiva per gli utenti.</p></li><li><p><strong>Feedback Sonoro:</strong> Ogni tratto o azione dell'utente può essere accompagnato da suoni interattivi, migliorando l'esperienza multisensoriale.</p></li></ol>
    <h3>Struttura del Codice:</h3>
    <p>Il codice sarà suddiviso in moduli principali come:</p>
    <ul class="list-disc list-inside p-5"><li><p><strong>Gestione del Kinect:</strong> Configurazione del sensore Kinect per rilevare il corpo e i movimenti.</p></li><li><p><strong>Grafica 3D:</strong> Creazione dello spazio virtuale in cui gli utenti possono disegnare.</p></li><li><p><strong>Gestione dell'Input:</strong> Traduzione dei dati del sensore Kinect in azioni di disegno sulla tela virtuale.</p></li><li><p><strong>Interfaccia Utente:</strong> Implementazione di un'interfaccia utente per la selezione dei colori e altre opzioni.</p></li><li><p><strong>Gestione del Suono:</strong> Integrazione di suoni interattivi in base alle azioni dell'utente.</p></li></ul>
    <h3>Esperienza Utente:</h3>
    <p>Gli utenti possono entrare nell'installazione e diventare artisti digitali, creando opere d'arte uniche con il loro corpo. Possono sperimentare con colori, movimenti e suoni, trasformando lo spazio circostante in una tela di espressione artistica interattiva.</p>
    <p>"KinectCanvas" offre un'esperienza unica che combina l'arte digitale, l'interazione corporea e l'immersione 3D per coinvolgere il pubblico in un'installazione interattiva e coinvolgente.</p>


  </BodyComponent>
<div>
    <div class="p-8 flex flex-1 items-center justify-center">    
      <iframe width="560" height="315" src="https://www.youtube.com/embed/videoseries?si=j3JHJnCYcox3bmgz&amp;list=PLvOBFN03LY9Qot3NxryszmQl1qZZ4r7gP" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
    </div>
    <div class="p-8 flex flex-1 items-center justify-center">    
      <iframe width="560" height="315" src="https://www.youtube.com/embed/xig1AzfaYv8?si=7zhhWSENVkuntrd0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
    </div>
    <div class="p-8 flex flex-1 items-center justify-center">    
      <iframe width="560" height="315" src="https://www.youtube.com/embed/tKUDLLA1Eek?si=0faITJIktKRvefRX" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
      </div>
     <div class="p-8 flex flex-1 items-center justify-center">    
      <iframe width="560" height="315" src="https://www.youtube.com/embed/BMduCeYiBQc?si=Wlz_t0IB5ce_z560" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
    </div>



</div>
</template>

