# Configuratore pannelli flessibili v2026 - online configurator 2026

> **Strumento web 2026 per configurare pannelli fotovoltaici flessibili e microinverter, con stime rapide per collegamenti, cablaggio e compatibilita essenziale.**

[![Platform](https://img.shields.io/badge/Platform-web-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-v2026-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/wardbenynr6229/configuratore-pannelli-flex-2026?style=flat-square)](https://github.com/wardbenynr6229/configuratore-pannelli-flex-2026)

---

<p align="center">
  <a href="https://wardbenynr6229.github.io/configuratore-pannelli-flex-2026/">
    <img src="https://img.shields.io/badge/Download-Configuratore%20pannelli%20flessibili%20Latest-brightgreen?style=for-the-badge" alt="Download Configuratore pannelli flessibili">
  </a>
</p>

> **[Download Configuratore pannelli flessibili v2026](https://wardbenynr6229.github.io/configuratore-pannelli-flex-2026/)**

---

[Download Latest Build](https://wardbenynr6229.github.io/configuratore-pannelli-flex-2026/)

---

## Panoramica

Configuratore pannelli flessibili e una web app per valutare la progettazione di impianti con pannelli fotovoltaici flessibili e microinverter. In base ai parametri inseriti, indica quanti pannelli possono essere collegati, propone la distribuzione dei collegamenti in serie e in parallelo e fornisce indicazioni sul cablaggio degli ingressi MPPT.

Il configuratore e pensato per controlli preliminari, confronti tra prodotti e prime fasi della progettazione. La logica viene eseguita in una struttura web statica basata su `data.json`, che consente di utilizzare sia sistemi preimpostati sia valori personalizzati per l'inverter tramite un'interfaccia leggera accessibile dal browser.

---

## Funzionalita principali

- Determina il numero di pannelli fotovoltaici flessibili collegabili ai microinverter supportati
- Confronta le configurazioni in serie e in parallelo per ogni ingresso MPPT
- Fornisce una stima della sezione dei cavi in funzione della distanza
- Include sistemi predefiniti per velocizzare la configurazione
- Permette di inserire manualmente i parametri di un inverter personalizzato
- Gestisce sistemi e collegamenti ai negozi tramite configurazione statica in `data.json`
- Funziona come applicazione web statica, distribuibile tramite un semplice hosting browser
- Supporta l'inserimento in iframe con comunicazione per il calcolo automatico dell'altezza

---

## Installazione e avvio

Il progetto non richiede una pipeline di build per l'utilizzo di base ed e progettato per essere servito come applicazione web statica.

1. Scarica i file del progetto o clona il repository:
   - `git clone https://github.com/wardbenynr6229/configuratore-pannelli-flex-2026.git
2. Pubblica i file su un servizio di hosting statico oppure avviali tramite un web server locale.
3. Apri la pagina HTML principale nel browser, oppure distribuisci la cartella nell'ambiente di hosting scelto.

Per le prove sul computer locale, e sufficiente usare un server statico semplice e visitare l'URL locale che verra indicato.

---

## Utilizzo

1. Avvia il configuratore in un browser moderno.
2. Scegli un sistema gia disponibile oppure inserisci i parametri dell'inverter manualmente.
3. Compila i dati relativi ai pannelli e all'installazione richiesti dal calcolo.
4. Controlla il numero di collegamenti suggerito, lo schema serie-parallelo e la stima della sezione dei cavi.
5. Modifica i valori fino a ottenere una configurazione coerente con l'impianto previsto.

Quando l'applicazione viene incorporata in un'altra pagina, inseriscila in un iframe e abilita la comunicazione prevista per l'auto-height, così il contenitore puo adattarsi all'altezza del contenuto.

---

## Dati e configurazione

Le impostazioni principali sono raccolte nel file statico `data.json`.

Struttura di esempio:

```json
{
  "systems": [],
  "storeLinks": []
}
```

Il file consente di definire i sistemi preimpostati, i riferimenti supportati e i link esterni ai negozi. In caso di personalizzazione, la struttura JSON deve restare compatibile con la logica utilizzata dall'interfaccia web.

---

## Requisiti

- Browser web moderno
- Hosting statico oppure accesso ai file tramite server o ambiente locale
- Supporto JSON per la configurazione `data.json`
- Nessun passaggio di build necessario per l'utilizzo di base
- Distribuibile come applicazione web basata su HTML statico

---

## Domande frequenti

**Come posso modificare i sistemi disponibili?**  
Aggiorna il file statico `data.json`, quindi pubblica nuovamente i file modificati.

**E possibile usare valori personalizzati per l'inverter?**  
Si. Oltre ai sistemi predefiniti, il configuratore consente di specificare parametri personalizzati dell'inverter.

**Posso incorporare l'applicazione in un altro sito?**  
Si. L'applicazione puo essere caricata in un iframe e comunica l'altezza necessaria per adattarsi al contenitore.

**Cosa devo controllare se i risultati non sembrano corretti?**  
Verifica i valori inseriti, il sistema selezionato e la configurazione JSON utilizzata dall'applicazione.

**Dove posso trovare la versione piu recente?**  
Usa il collegamento per il download riportato sopra oppure recupera i file aggiornati dal repository del progetto.

---

## Licenza

GNU GPL v3.0 - consulta [LICENSE](LICENSE) per i dettagli.
