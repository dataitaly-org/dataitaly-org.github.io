---
title: "Trasparenza e Accessibilità dei Dati COVID-19 in Italia"
date: 2024-01-01
---

## Trasparenza nella pubblicazione dei dati COVID-19

La pandemia da Covid-19, oltre ad aver sconvolto le nostre vite, ha posto nuove sfide in termini di trasparenza nella pubblicazione dei dati da parte dei governi di tutto il mondo. Infatti, per non cadere nella trappola di argomentazioni e tesi lontane dalla realtà, è indispensabile consentire ai cittadini di avere accesso tempestivo alle stesse informazioni utilizzate per giustificare l'inasprimento o l'allentamento delle restrizioni alle libertà personali per fini sanitari.

Sin dall'inizio dello stato d'emergenza, diverse pubbliche amministrazioni italiane hanno realizzato delle utili raccolte di dati [di tipo aperto](https://www.agid.gov.it/it/dati/open-data) messe a disposizione del pubblico per analisi e studi statistici.

### Dati COVID-19 Italia

Il dataset **Dati COVID-19 Italia** è pubblicato ed aggiornato giornalmente, a partire dal 7 marzo 2020, dal Dipartimento della Protezione Civile ed è consultabile presso il seguente repository GitHub secondo i termini della licenza [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/): [https://github.com/pcm-dpc/COVID-19](https://github.com/pcm-dpc/COVID-19). La pubblicazione è diventata settimanale a partire da novembre 2022.

Le serie di dati hanno inizio il giorno 24 febbraio 2020 e sono disponibili in formato JSON e CSV. A livello di regione sono disponibili, per ogni giorno, il numero di tamponi effettuati ed il totale dei casi, il numero degli attualmente positivi (pari al numero di ospedalizzati più il numero di soggetti in isolamento), il numero di guariti ed il numero di deceduti. A livello di provincia, sempre con granularità giornaliera, è disponibile solo il totale di casi, ma non gli altri dati. Non è invece prevista la pubblicazione di alcun dato a livello di comune.

Per maggiori dettagli sul significato dei vari campi si può consultare lo [schema dei dati](https://github.com/pcm-dpc/COVID-19/blob/master/dati-andamento-covid19-italia.md) disponibile nello stesso repository. Sulla base di questo dataset, il Ministero della Salute realizza la scheda [Aggiornamento casi Covid-19](https://raw.githubusercontent.com/pcm-dpc/COVID-19/master/schede-riepilogative/regioni/dpc-covid19-ita-scheda-regioni-latest.pdf) spesso rilanciata da diversi organi di informazione.

{{< chart id="positivi" type="line" csvfile="covid/positivi.csv" title="Numero di positivi per data" >}}

{{< chart id="ospedalizzati" type="line" csvfile="covid/ospedalizzati.csv" title="Numero di ospedalizzati per data" >}}

### Dati della Sorveglianza integrata COVID-19

L'Istituto Superiore di Sanità (ISS) pubblica invece i **Dati della Sorveglianza integrata COVID-19** all'interno di un cruscotto informativo ed in un file Excel disponibili presso: [https://www.epicentro.iss.it/coronavirus/sars-cov-2-dashboard](https://www.epicentro.iss.it/coronavirus/sars-cov-2-dashboard). Da settembre 2023 l'ISS ha cambiato la frequenza di aggiornamento dei dati della sorveglianza integrata COVID-19 a cadenza settimanale (ogni giovedì) e ha eliminato alcuni fogli dati dai suoi open data.

Questi dati sono leggermente differenti rispetto a quelli pubblicati dalla Protezione Civile perché seguono un flusso informativo diverso. Come spiegato nelle FAQ del [Sistema di sorveglianza integrata COVID-19](https://www.epicentro.iss.it/coronavirus/sars-cov-2-sorveglianza), l'ISS raccoglie i dati completi di ogni caso, compresi quindi i dati demografici e la storia clinica del paziente, mentre la Protezione Civile gestisce solo dati già aggregati all'origine, raccolti con frequenza giornaliera. Per questo motivo i dati dell'ISS, naturalmente sempre pubblicati in forma aggregata, sono disponibili con alcuni giorni di ritardo.

### Immuni Open Data

La Presidenza del Consiglio dei Ministri ha pubblicato, con licenza [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/), il dataset **Immuni Open Data** relativo ai download ed alle notifiche inviate dall'app [Immuni](https://www.immuni.italia.it/) presso il seguente repository GitHub: [https://github.com/immuni-app/immuni-dashboard-data](https://github.com/immuni-app/immuni-dashboard-data). A partire dal 31 dicembre 2022 l'app Immuni non è più disponibile nei negozi di applicazioni mobili e non funziona più sui dispositivi su cui è stata installata. Tutti i repository associati sono stati archiviati in modalità sola lettura.

Nel dettaglio, sono disponibili i dati giornalieri relativi ai download dell'applicazione per piattaforma (Android e iOS), il numero giornaliero di utenti positivi e notifiche inviate a livello nazionale, ed il numero settimanale e mensile di utenti positivi e notifiche inviate a livello regionale. Il numero delle notifiche inviate è tuttavia parziale, perché non tutti i dispositivi Android permettono di raccogliere questa informazione in modo sicuro. Come per il dataset **Dati COVID-19 Italia**, i dati sono disponibili in formato JSON e CSV ed aggiornati giornalmente fino alla chiusura del progetto.

### Covid-19 Opendata Vaccini

Sempre la Presidenza del Consiglio dei Ministri pubblica, con licenza [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/), il dataset **Covid-19 Opendata Vaccini** contenente il numero di dosi di vaccini somministrati nel seguente repository GitHub: [https://github.com/italia/covid19-opendata-vaccini](https://github.com/italia/covid19-opendata-vaccini).

In questo dataset sono disponibili i numeri di dosi di vaccini consegnate dalla struttura commissariale per giorno, fornitore e regione, il numero di dosi consegnate e somministrate per regione, l'elenco dei punti di somministrazione ed il numero di prime e seconde dosi somministrate per data, regione, fascia anagrafica e sesso. Anche in questo caso i dati sono disponibili in formato JSON e CSV e sono aggiornati ogni giorno fino a novembre 2023, quindi l'aggiornamento è diventato settimanale. Gli stessi dati in forma aggregata si possono anche consultare nel cruscotto [Report Vaccini Anti COVID-19](https://www.governo.it/it/cscovid19/report-vaccini/).

### Numero di vaccinati e ospedalizzati per data

Incrociando diversi dataset, con le dovute cautele, è possibile effettuare ulteriori confronti di potenziale interesse. Per esempio, utilizzando i dataset **Dati COVID-19 Italia** e **Covid-19 Opendata Vaccini** è possibile realizzare la seguente visualizzazione relativa al numero di vaccinati e ospedalizzati per data.
