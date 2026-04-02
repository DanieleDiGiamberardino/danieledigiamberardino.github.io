---
layout: page
name: Architettura e Interfacce Custom in ROS 2 per Videocamere PTZ
tools: [ROS 2, Architettura Software, Custom Messages, Sensori]
image: "" 
description: Progettazione dell'architettura ROS 2 e sviluppo di interfacce di comunicazione personalizzate per il controllo e l'acquisizione video da videocamere PTZ.
---

<div class="row mt-5">
  
  <div class="col-md-7">
    <h3 class="mb-4">L'Obiettivo Architetturale</h3>
    <p class="text-justify">
      In sistemi robotici complessi, la standardizzazione della comunicazione è vitale. L'obiettivo di questo progetto è stato quello di creare le fondamenta strutturali (in ambiente <strong>ROS 2</strong>) per l'interfacciamento con videocamere motorizzate <strong>PTZ (Pan-Tilt-Zoom)</strong>.
    </p>

    <h3 class="mt-5 mb-4">Sviluppo delle Interfacce (Custom Messages)</h3>
    <p>Il lavoro si è concentrato sulla definizione dei pacchetti e dei protocolli di comunicazione, sviluppando messaggi personalizzati per sincronizzare l'acquisizione visiva con il controllo hardware. Nello specifico abbiamo strutturato:</p>
    
    <ul class="list-group list-group-flush mb-4">
      <li class="list-group-item bg-transparent border-0 pl-0"><i class="fas fa-network-wired text-primary mr-2"></i> <strong>Gestione PTZF:</strong> Definizione dei messaggi per il controllo di Pan, Tilt, Zoom e Focus.</li>
      <li class="list-group-item bg-transparent border-0 pl-0"><i class="fas fa-layer-group text-primary mr-2"></i> <strong>Sincronizzazione Dati:</strong> Creazione di messaggi compositi per accoppiare in tempo reale il flusso video (<code>sensor_msgs/Image</code>) con la posa attuale della videocamera.</li>
      <li class="list-group-item bg-transparent border-0 pl-0"><i class="fas fa-project-diagram text-primary mr-2"></i> <strong>Setup del Workspace:</strong> Configurazione delle dipendenze C++ (OpenCV, Image Transport) per i futuri nodi di elaborazione.</li>
    </ul>
  </div>

  <div class="col-md-5 mt-4 mt-md-0">
    <div class="card shadow-sm border-0 bg-light p-3">
       <h6 class="text-muted mb-3"><i class="fas fa-code"></i> Esempio: ImagePTZF.msg</h6>
       
       <pre class="bg-dark text-light p-3 rounded" style="font-size: 0.85em;"><code># Camera image, with pan-tilt-zoom values.

# Current frame
sensor_msgs/Image image

# Current PTZF values
PTZF ptzf</code></pre>

       <p class="small text-muted mt-3 mb-0">Il messaggio custom che accoppia in un unico topic il frame video e i parametri cinematici della videocamera.</p>
    </div>
  </div>
</div>
