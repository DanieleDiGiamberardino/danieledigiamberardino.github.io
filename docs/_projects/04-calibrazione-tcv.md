---
layout: page
name: Calibrazione Adattiva RLS per Sensori Tokamak (TCV)
tools: [Ottimizzazione RLS, Elaborazione Segnali, Sensor Fusion, MATLAB]
image: ../schema-diagnostic-tcv.png
description: Sviluppo di un algoritmo ai Minimi Quadrati Ricorsivi (RLS) per la calibrazione dinamica incrociata di diodi AXUV e bolometri in reattori a fusione nucleare.
---

<div class="row mt-5">
  
  <div class="col-md-7">
    <h3 class="mb-4">Contesto Operativo</h3>
    <p class="text-justify">
      Nel controllo del plasma all'interno dei reattori <strong>Tokamak</strong>, il monitoraggio della potenza dissipata è cruciale. I sensori tradizionali (bolometri) hanno tempi di risposta troppo lenti (millisecondi) per rilevare dinamiche instabili veloci come gli <strong>ELMs</strong>. I diodi AXUV risolvono il problema della velocità (microsecondi), ma presentano lo svantaggio di non poter essere calibrati in maniera assoluta.
    </p>

    <h3 class="mt-5 mb-4">La Soluzione Algoritmica</h3>
    <p>Per superare questo limite hardware, ho contribuito allo sviluppo di un modello di calibrazione lineare iterativo basato sull'algoritmo di ottimizzazione <strong>RLS (Recursive Least Squares)</strong>. Il lavoro si è articolato in diverse fasi:</p>
    
    <ul class="list-group list-group-flush mb-4">
      <li class="list-group-item bg-transparent border-0 pl-0"><i class="fas fa-filter text-primary mr-2"></i> <strong>Data Pre-processing:</strong> Filtraggio del rumore e interpolazione spaziale/temporale per mitigare le misurazioni errate derivanti da Linee di Vista (LOS) malfunzionanti (mostrate nello schema a destra).</li>
      <li class="list-group-item bg-transparent border-0 pl-0"><i class="fas fa-sync text-primary mr-2"></i> <strong>Stima Adattiva (RLS):</strong> Implementazione dell'aggiornamento iterativo della stima dei parametri, della matrice di covarianza (incertezza) e del guadagno.</li>
      <li class="list-group-item bg-transparent border-0 pl-0"><i class="fas fa-chart-area text-primary mr-2"></i> <strong>Cross-Calibration:</strong> Utilizzo dell'emissività ricostruita dai bolometri come riferimento base per calibrare dinamicamente le misure dei diodi AXUV ad alta frequenza.</li>
    </ul>
  </div>

  <div class="col-md-5 mt-4 mt-md-0 text-center">
    <img src="../schema-diagnostic-tcv.png" alt="Schema Geometrico Linee di Vista TCV" class="img-fluid rounded shadow-sm mb-4">
    
    <div class="card shadow-sm border-0 bg-light p-4 text-center">
       <i class="fas fa-bolt fa-3x text-secondary mb-3"></i>
       <h5 class="text-muted">Risultati Ottenuti</h5>
       <p class="small text-muted mt-2 mb-3">La calibrazione ha permesso ai diodi AXUV di ricostruire con successo i picchi di instabilità veloce (ELMs) che i bolometri non riuscivano a rilevare per via della loro limitata risoluzione temporale, garantendo un'ottima ricostruzione dell'emissività.</p>
       
       <a href="../Tesina_Cross_Calibration.pptx" class="btn btn-outline-primary btn-sm"><i class="fas fa-file-powerpoint mr-2"></i> Presentazione Progetto</a>
    </div>
  </div>
</div>
