---
layout: page
name: Controllo di Assetto (TVC) per Razzi Modello
tools: [MATLAB, Simulink, Controllo PID, Dinamica Aerospaziale, AI-Assisted]
image: https://images.unsplash.com/photo-1517976487492-5750f3195933?ixlib=rb-1.2.1&auto=format&fit=crop&w=800&q=80
description: "WORK IN PROGRESS: Progettazione e implementazione di un sistema di controllo ad anello chiuso (PID) per la stabilizzazione tramite Thrust Vector Control in Simulink."
---

<div class="row mt-5">
  
  <div class="col-md-7">
    <h3 class="mb-4">Il Progetto e la Sfida (WIP) 🚀</h3>
    <p class="text-justify">
      La stabilizzazione di un razzo in volo è un classico problema di controllo del pendolo inverso, reso estremamente complesso dalle dinamiche aerospaziali e dalle repentine variazioni di massa. Questo progetto personale, attualmente in fase di sviluppo, punta a implementare il sistema di controllo per l'assetto di un razzo modello.
    </p>

    <h3 class="mt-5 mb-4">Sviluppo e Chiusura dell'Anello</h3>
    <p>Partendo da un accurato modello fisico matematico <em>open-loop</em> (sviluppato e ispirato dalla community aerospaziale BPS.space), il mio lavoro si sta concentrando sulla progettazione della retroazione:</p>
    
    <ul class="list-group list-group-flush mb-4">
      <li class="list-group-item bg-transparent border-0 pl-0"><i class="fas fa-rocket text-primary mr-2"></i> <strong>Dinamica 3-DOF:</strong> Sfruttamento del modello fisico che tiene conto di massa, momenti d'inerzia e risoluzione trigonometrica dei vettori di spinta.</li>
      <li class="list-group-item bg-transparent border-0 pl-0"><i class="fas fa-project-diagram text-primary mr-2"></i> <strong>Sviluppo Closed-Loop:</strong> Progettazione dell'architettura di controllo tramite l'inserimento di <strong>due controllori PID indipendenti</strong> per comandare dinamicamente il <em>Thrust Vector Control (TVC)</em> sui vari assi in base all'errore di assetto.</li>
      <li class="list-group-item bg-transparent border-0 pl-0"><i class="fas fa-robot text-primary mr-2"></i> <strong>AI-Assisted Development:</strong> Utilizzo di Large Language Models (LLM) come supporto attivo allo sviluppo, per il troubleshooting avanzato in ambiente Simulink e il supporto nel tuning dei parametri.</li>
    </ul>
  </div>

  <div class="col-md-5 mt-4 mt-md-0 text-center">
    <img src="https://images.unsplash.com/photo-1517976487492-5750f3195933?ixlib=rb-1.2.1&auto=format&fit=crop&w=800&q=80" alt="Rocket Launch" class="img-fluid rounded shadow-sm mb-4">
    
    <div class="card shadow-sm border-0 bg-light p-4 text-center" style="border-left: 4px solid #ffc107 !important;">
       <i class="fas fa-tools fa-3x text-warning mb-3"></i>
       <h5 class="text-muted">Work in Progress</h5>
       <p class="small text-muted mt-2 mb-0">Il modello Simulink è in fase di calibrazione e ottimizzazione del PID. Ritengo che lavorare a progetti personali extra-curriculari e affrontare le difficoltà della sintonizzazione (tuning) su sistemi non lineari sia il modo migliore per rafforzare le proprie competenze ingegneristiche sul campo.</p>
    </div>
  </div>
</div>
