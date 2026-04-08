---
layout: page
name: Software gestionale (Sviluppo personale) (WIP)
tools: [Python, CustomTkinter, OpenCV, SQLite, AI-Assisted Dev]
image: https://images.unsplash.com/photo-1576091160550-2173dba999ef?ixlib=rb-1.2.1&auto=format&fit=crop&w=800&q=80
description: Sviluppo di un'applicazione desktop in python per l'archiviazione strutturata di foto cliniche e la gestione dei pazienti in ambito odontoiatrico.
---

<div class="row mt-5">
  
  <div class="col-md-7">
    <h3 class="mb-4">Il Progetto (Sviluppo personale)</h3>
    <p class="text-justify">
      Oltre ai progetti puramente ingegneristici, mi dedico allo sviluppo di software completi per risolvere problemi reali (per imparare a risolvere diverse problematiche). Attualmente sto sviluppando da zero un'applicazione gestionale desktop per studi odontoiatrici, focalizzata sull'organizzazione del database fotografico clinico dei pazienti.
    </p>

    <h3 class="mt-5 mb-4">Architettura e funzionalità software</h3>
    <p>Il progetto è un'applicazione modulare scritta in Python, che fa largo uso del paradigma object-oriented e integra librerie avanzate. Lo sviluppo è stato supportato dall'utilizzo di <strong>modelli linguistici (LLM)</strong> per accelerare la prototipazione e il refactoring del codice.</p>
    
    <ul class="list-group list-group-flush mb-4">
      <li class="list-group-item bg-transparent border-0 pl-0"><i class="fas fa-desktop text-primary mr-2"></i> <strong>Interfaccia grafica:</strong> Sviluppo di una GUI moderna multi-frame con <em>CustomTkinter</em>, comprensiva di sistema di login, cruscotto statistico e visualizzatore immagini con pan/zoom dinamico.</li>
      <li class="list-group-item bg-transparent border-0 pl-0"><i class="fas fa-camera text-primary mr-2"></i> <strong>Integrazione hardware:</strong> Utilizzo di <em>openCV</em> per il controllo delle webcam e sviluppo di un demone asincrono (<em>watchdog</em>) per l'auto-import in tempo reale di immagini da fotocamere esterne.</li>
      <li class="list-group-item bg-transparent border-0 pl-0"><i class="fas fa-database text-primary mr-2"></i> <strong>Gestione dati:</strong> Architettura basata su database (SQLite) per l'associazione delle immagini alle schede paziente, con tagging strutturato (dente, branca, fase) e generazione di timeline cliniche.</li>
    </ul>
  </div>

  <div class="col-md-5 mt-4 mt-md-0 text-center">
    <img src="https://images.unsplash.com/photo-1576091160550-2173dba999ef?ixlib=rb-1.2.1&auto=format&fit=crop&w=800&q=80" alt="Gestione clinica" class="img-fluid rounded shadow-sm mb-4">
    
    <div class="card shadow-sm border-0 bg-light p-4 text-center">
       <i class="fas fa-laptop-code fa-3x text-secondary mb-3"></i>
       <h5 class="text-muted">Stato del progetto</h5>
       <p class="small text-muted mt-2 mb-3">Il progetto è attualmente in fase di sviluppo (Work In Progress). Il core dell'applicazione (upload, formattazione dati e UI principale) è operativo, mentre sono in fase di test le procedure di importazione massiva e il backup di sicurezza.</p>
       
       <button class="btn btn-outline-secondary btn-sm" disabled><i class="fab fa-github mr-2"></i> Repository privato</button>
    </div>
  </div>
</div>
