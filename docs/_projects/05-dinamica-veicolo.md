---
layout: page
name: Analisi vibrazionale e modellistica automotive (Quarter-Car)
tools: [MATLAB, Simulink, Arduino, Dinamica del Veicolo]
image: https://images.unsplash.com/photo-1486262715619-67b85e0b08d3?ixlib=rb-1.2.1&auto=format&fit=crop&w=800&q=80
description: Acquisizione sperimentale di dati telemetrici e modellazione in Simulink per lo studio delle vibrazioni verticali di un veicolo ibrido.
---

<div class="row mt-5">
  
  <div class="col-md-7">
    <h3 class="mb-4">Il Progetto Sperimentale</h3>
    <p class="text-justify">
      Nell'industria Automotive, la validazione dei modelli matematici tramite prove su strada è fondamentale per lo sviluppo di sospensioni attive e sistemi di comfort. Questo progetto si è concentrato sull'analisi delle vibrazioni verticali di un veicolo ibrido sottoposto a diversi profili stradali (strada liscia e sterrata).
    </p>

    <h3 class="mt-5 mb-4">Hardware e Modellazione in Simulink</h3>
    <p>Il lavoro ha unito l'acquisizione pratica dei dati alla simulazione al calcolatore, articolandosi in:</p>
    
    <ul class="list-group list-group-flush mb-4">
      <li class="list-group-item bg-transparent border-0 pl-0"><i class="fas fa-microchip text-primary mr-2"></i> <strong>Telemetria e Sensori:</strong> Progettazione di un sistema di acquisizione basato su Arduino UNO e sensore inerziale (IMU MPU6050) posizionato nel baricentro del veicolo.</li>
      <li class="list-group-item bg-transparent border-0 pl-0"><i class="fas fa-laptop-code text-primary mr-2"></i> <strong>Digital Twin (Simscape):</strong> Creazione di modelli fisici in ambiente Simulink per simulare la risposta dinamica del sistema.</li>
      <li class="list-group-item bg-transparent border-0 pl-0"><i class="fas fa-chart-line text-primary mr-2"></i> <strong>Validazione 1-DOF vs 2-DOF:</strong> Analisi comparativa per dimostrare l'insufficienza di un modello a singolo grado di libertà e la necessità di un modello <em>Quarter-Car</em> (2-DOF) per descrivere l'interazione tra massa sospesa e non sospesa.</li>
    </ul>
  </div>

  <div class="col-md-5 mt-4 mt-md-0 text-center">
    <img src="https://images.unsplash.com/photo-1486262715619-67b85e0b08d3?ixlib=rb-1.2.1&auto=format&fit=crop&w=800&q=80" alt="Dinamica del Veicolo" class="img-fluid rounded shadow-sm mb-4">
    
    <div class="card shadow-sm border-0 bg-light p-4 text-center">
       <i class="fas fa-car-side fa-3x text-secondary mb-3"></i>
       <h5 class="text-muted">Esito dell'Analisi</h5>
       <p class="small text-muted mt-2 mb-3">L'analisi nel dominio del tempo e della frequenza ha confermato che il modello 2-DOF replica con estrema precisione i dati reali acquisiti su strada. Lo studio matematico ha inoltre validato la stabilità asintotica di entrambi i modelli.</p>
       
       <a href="../Meccanica_delle_Vibrazioni.pdf" class="btn btn-outline-primary btn-sm"><i class="fas fa-file-pdf mr-2"></i> Scarica Presentazione</a>
    </div>
  </div>
</div>
