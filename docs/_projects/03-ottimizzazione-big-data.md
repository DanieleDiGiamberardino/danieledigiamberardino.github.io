---
layout: page
name: Ottimizzazione per Big Data e Deep Learning
tools: [MATLAB, Machine Learning, Ottimizzazione, Reti Neurali]
image: https://images.unsplash.com/photo-1551288049-bebda4e38f71?ixlib=rb-1.2.1&auto=format&fit=crop&w=800&q=80
description: Sviluppo da zero di reti neurali per la classificazione di dataset complessi, con implementazione di algoritmi di ottimizzazione e cross-validation in MATLAB.
---

<div class="row mt-5">
  
  <div class="col-md-7">
    <h3 class="mb-4">Il Progetto e i Dati</h3>
    <p class="text-justify">
      In questo progetto ci siamo concentrati sull'implementazione matematica e sull'ottimizzazione di <strong>Reti neurali</strong> da zero, applicate a problemi di classificazione binaria e multiclasse su dataset di grandi dimensioni (RNA e Shuttle).
    </p>

    <h3 class="mt-5 mb-4">Sviluppo in MATLAB e architettura</h3>
    <p>Abbiamo sviluppato la pipeline di apprendimento scrivendo manualmente le funzioni core, tra cui:</p>
    
    <ul class="list-group list-group-flush mb-4">
      <li class="list-group-item bg-transparent border-0 pl-0"><i class="fas fa-brain text-primary mr-2"></i> <strong>Core network:</strong> Implementazione di forward e back-propagation per il calcolo dei gradienti, con funzioni di attivazione ReLU e SoftMax.</li>
      <li class="list-group-item bg-transparent border-0 pl-0"><i class="fas fa-chart-line text-primary mr-2"></i> <strong>Metodi di ottimizzazione:</strong> Utilizzo dell'anti-gradiente come direzione di discesa e calcolo dinamico del passo di aggiornamento tramite il <strong>Metodo di armijo</strong> per garantire la convergenza.</li>
      <li class="list-group-item bg-transparent border-0 pl-0"><i class="fas fa-filter text-primary mr-2"></i> <strong>Tuning e prevenzione overfitting:</strong> Inizializzazione dei pesi con metodo <em>He</em>, applicazione della regolarizzazione L2 e procedure di cross-validation per ottimizzare il numero di layer e neuroni.</li>
    </ul>
  </div>

  <div class="col-md-5 mt-4 mt-md-0">
    <img src="https://images.unsplash.com/photo-1551288049-bebda4e38f71?ixlib=rb-1.2.1&auto=format&fit=crop&w=800&q=80" alt="Data Analytics" class="img-fluid rounded shadow-sm mb-4">
    
    <div class="card shadow-sm border-0 bg-light p-4 text-center">
       <i class="fas fa-code-branch fa-3x text-secondary mb-3"></i>
       <h5 class="text-muted">Risultati</h5>
       <p class="small text-muted mt-2 mb-3">Le configurazioni testate hanno dimostrato un'eccellente capacità di generalizzazione, mitigando l'overfitting al crescere della complessità della rete e mantenendo un'alta accuratezza sia sul Validation che sul Test set.</p>
       
       <a href="../Relazione_Progetto_OBD.docx" class="btn btn-outline-primary btn-sm"><i class="fas fa-file-word mr-2"></i> Report Completo</a>
    </div>
  </div>
</div>
