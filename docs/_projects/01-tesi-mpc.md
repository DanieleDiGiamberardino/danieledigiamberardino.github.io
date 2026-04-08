---
layout: page
name: Model Predictive Control con Metodi Data-Driven e Reti Neurali
tools: [MATLAB, Python, Deep Learning, Controllo Avanzato]
image: ../mpc-vehicle-model.png
description: Sviluppo di logiche di controllo predittivo ibride per l'ottimizzazione di sistemi dinamici complessi, unendo teoria del controllo e intelligenza artificiale.
---

<div class="row mt-5">
  
  <div class="col-md-8">
    <h3 class="mb-4">Obiettivo del Progetto</h3>
    <p class="text-justify">
      L'obiettivo principale di questo lavoro di tesi è stato progettare e implementare un sistema di <strong>Model Predictive Control (MPC)</strong> capace di superare i limiti della modellistica matematica classica, integrandola con approcci <em>data-driven</em>.
    </p>

    <h3 class="mt-5 mb-4">Metodologia e Tecnologie</h3>
    <p>Per gestire dinamiche complesse e non lineari, ho affiancato la teoria del controllo ottimo all'utilizzo di <strong>Reti neurali</strong>. L'architettura sviluppata permette al sistema di:</p>
    
    <ul class="list-group list-group-flush mb-4">
      <li class="list-group-item bg-transparent border-0 pl-0"><i class="fas fa-check-circle text-primary mr-2"></i> Apprendere il comportamento dinamico dell'impianto direttamente dai dati storici.</li>
      <li class="list-group-item bg-transparent border-0 pl-0"><i class="fas fa-check-circle text-primary mr-2"></i> Poter ricostruire la funzione di costo associata al modello per il task d'inseguimento asintotico</li>
      <li class="list-group-item bg-transparent border-0 pl-0"><i class="fas fa-check-circle text-primary mr-2"></i> Calcolare l'azione di controllo ottima garantendo stabilità e rispetto dei vincoli.</li>
    </ul>

    <h3 class="mt-5 mb-4">Applicazioni Pratiche</h3>
    <p class="text-justify">
      Questo approccio ibrido rappresenta lo stato dell'arte per l'Automazione Moderna. La soluzione sviluppata è pensata per essere scalabile e applicabile a progetti industriali concreti, dalla robotica avanzata alla gestione energetica di impianti complessi.
    </p>
  </div>

  <div class="col-md-4 mt-4 mt-md-0 text-center">
    
    <img src="../mpc-vehicle-model.png" alt="Schema MPC" class="img-fluid rounded shadow-sm mb-5">
    
    <div class="card shadow-sm border-0 bg-light">
      <div class="card-body">
        <h5 class="card-title mb-4">Documentazione</h5>
        <a href="../tesi-mpc-digiamberardino.pdf" class="btn btn-primary btn-block mb-3" target="_blank">
          <i class="fas fa-file-pdf mr-2"></i> Scarica la Tesi
        </a>
        <a href="../presentazione-mpc.pptx" class="btn btn-outline-primary btn-block" target="_blank">
          <i class="fas fa-file-powerpoint mr-2"></i> Presentazione
        </a>
      </div>
    </div>

  </div>
</div>
