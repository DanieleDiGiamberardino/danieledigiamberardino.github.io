---
layout: page
name: Stabilizzazione Pendolo Inverso
tools: [MATLAB, Arduino, C++, Controllo Classico]
image: docs/pendulum.png
description: Progettazione e implementazione fisica di un sistema di controllo ad anello chiuso per la stabilizzazione di un pendolo inverso tramite controllori di stato sintetizzati in MATLAB e implementati su hardware Arduino.
---

<div class="row mt-5">
  
  <div class="col-md-8">
    <h3 class="mb-4">Obiettivo del progetto</h3>
    <p class="text-justify">
      L'obiettivo del progetto è stato progettare e implementare fisicamente un sistema di controllo capace di stabilizzare un <strong>pendolo inverso</strong> nel suo punto di equilibrio instabile — la posizione verticale — in presenza di perturbazioni esterne applicate direttamente all'asta.
    </p>

    <h3 class="mt-5 mb-4">Modellistica e linearizzazione</h3>
    <p class="text-justify">
      Il primo passo è stato derivare le equazioni del moto tramite la formulazione di <strong>Eulero-Lagrange</strong>, ottenendo un modello non lineare del sistema. Le equazioni sono state successivamente <strong>linearizzate attorno al punto di lavoro instabile</strong> (posizione verticale), ricavando un modello SISO utilizzabile per la sintesi del controllore. La variabile di uscita misurata è l'angolo dell'asta, acquisita tramite un <strong>giroscopio</strong> posizionato alla base del pendolo.
    </p>

    <h3 class="mt-5 mb-4">Sintesi del controllore e implementazione</h3>
    <p>Il flusso di sviluppo ha seguito le seguenti fasi:</p>
    
    <ul class="list-group list-group-flush mb-4">
      <li class="list-group-item bg-transparent border-0 pl-0"><i class="fas fa-check-circle text-primary mr-2"></i> Sintesi del controllore in MATLAB tramite analisi del <strong>diagramma di Bode</strong> e luogo delle radici.</li>
      <li class="list-group-item bg-transparent border-0 pl-0"><i class="fas fa-check-circle text-primary mr-2"></i> Conversione del controllore da tempo continuo a discreto e implementazione in <strong>C++ su microcontrollore Arduino</strong>.</li>
      <li class="list-group-item bg-transparent border-0 pl-0"><i class="fas fa-check-circle text-primary mr-2"></i> Attuazione tramite <strong>ponte H</strong> per il controllo del carrello sottostante al pendolo.</li>
      <li class="list-group-item bg-transparent border-0 pl-0"><i class="fas fa-check-circle text-primary mr-2"></i> Raccolta di dati sperimentali reali e <strong>tuning iterativo</strong> dei parametri del controllore e del modello (es. massa effettiva del pendolo).</li>
    </ul>

    <h3 class="mt-5 mb-4">Risultati</h3>
    <p class="text-justify">
      Il sistema implementato è in grado di mantenere stabilmente il pendolo in posizione verticale, reagendo in tempo reale alle perturbazioni applicate manualmente sull'asta. Il processo di identificazione sperimentale dei parametri ha permesso di colmare il gap tra il modello teorico e il comportamento reale del sistema fisico.
    </p>
    
  </div>

  <div class="col-md-4 mt-4 mt-md-0 text-center">
    
    <img src="../pendolo.jpg" alt="Pendolo Inverso" class="img-fluid rounded shadow-sm mb-5">
    
    <div class="card shadow-sm border-0 bg-light">
      <div class="card-body">
        <h5 class="card-title mb-4">Dettagli tecnici</h5>
        <ul class="list-unstyled text-left">
          <li class="mb-2"><i class="fas fa-microchip mr-2 text-primary"></i> Microcontrollore: Arduino</li>
          <li class="mb-2"><i class="fas fa-tachometer-alt mr-2 text-primary"></i> Sensore: Giroscopio IMU</li>
          <li class="mb-2"><i class="fas fa-bolt mr-2 text-primary"></i> Attuatore: Ponte H + motore DC</li>
          <li class="mb-2"><i class="fas fa-code mr-2 text-primary"></i> Linguaggi: MATLAB, C++</li>
        </ul>
      </div>
    </div>
        <!-- Sezione Presentazione aggiunta qui -->
    <div class="mt-5">
      <a href="../CA.pptx" class="btn btn-primary" download>
        <i class="fas fa-file-powerpoint mr-2"></i> Scarica la Presentazione (PPTX)
      </a>
    </div>
  </div>
</div>
