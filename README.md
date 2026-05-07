# 📚 Appunti di Laboratorio di Fisica 3

Questo repository contiene il codice sorgente in LaTeX per la stesura, la revisione e la condivisione degli appunti di Laboratorio 3 (Corso di Laurea in Fisica, Università di Catania) scritti dalla Dott.ssa Virginia Marchetta.

Per aggirare i limiti di tempo nella compilazione di file di grandi dimensioni imposti dalle versioni gratuite di piattaforme come Overleaf o Prism, abbiamo strutturato il progetto su **GitHub**. In questo modo, ognuno lavorerà in locale, sfruttando la potenza del proprio computer per generare i PDF, e sincronizzerà le modifiche tramite Git.

Di seguito trovi la guida completa per configurare il tuo ambiente di lavoro da zero.

---

## 🛠️ 1. Preparazione dell'Ambiente (Solo la prima volta)

Per poter collaborare a questo progetto, il tuo computer deve avere tre componenti fondamentali. Installali in quest'ordine:

1. **Il Compilatore LaTeX (Il Motore)**
   Senza questo, il computer non sa come trasformare il codice in un PDF.
   * **Windows:** Scarica e installa [MiKTeX](https://miktex.org/download/). (Assicurati di installarlo per tutti gli utenti se richiesto).
   * **macOS:** Scarica e installa [MacTeX](https://lukas-reineke.github.io/mactex/). È un file pesante, richiede un po' di tempo.
   * **Linux:** Apri il terminale e digita `sudo apt install texlive-full`.

2. **Git (Il Sistema di Controllo Versione)**
   Serve per scaricare i file dal server e caricare le tue modifiche.
   * Scarica [Git](https://git-scm.com/downloads) e procedi con l'installazione mantenendo tutte le opzioni predefinite.

3. **Visual Studio Code (L'Editor)**
   Il programma dove scriveremo effettivamente il codice.
   * Scarica e installa [VS Code](https://code.visualstudio.com/).

---

## ⚙️ 2. Configurazione di VS Code e Git

Una volta installati i programmi, dobbiamo collegarli tra loro.

### A. Installare l'estensione per LaTeX
1. Apri VS Code.
2. Vai nella scheda **Extensions** (l'icona con i 4 quadrati nel menu di sinistra, o premi `Ctrl+Shift+X`).
3. Cerca l'estensione **LaTeX Workshop** (creata da James Yu) e clicca su *Install*. Questo ti permetterà di avere il syntax highlighting e l'anteprima del PDF integrata.

### B. Identificarsi su Git
Git ha bisogno di "firmare" le tue modifiche per sapere chi ha scritto cosa.
1. In VS Code, apri il terminale integrato cliccando in alto su `Terminal` > `New Terminal`.
2. Digita questi due comandi, sostituendo i tuoi dati reali e premendo *Invio* dopo ciascuno:
   ```bash
   git config --global user.name "Il Tuo Nome e Cognome"
   git config --global user.email "la-tua-email@esempio.com" 

## 📥 3. Clonare il Repository

Ora devi scaricare l'intera cartella del progetto sul tuo PC. Non usare il tasto "Download ZIP", altrimenti perderai il collegamento con GitHub.

1. Vai sulla pagina GitHub di questo repository, clicca sul tasto verde **<> Code** e copia l'URL fornito.
2. Apri VS Code, premi `Ctrl + Shift + P` (o `Cmd + Shift + P` su Mac) per aprire la Command Palette.
3. Scrivi **Git: Clone** e premi Invio.
4. Incolla l'URL copiato e premi Invio.
5. Seleziona una cartella sul tuo PC dove vuoi salvare gli appunti.
6. Quando VS Code ti chiede se vuoi aprire il repository clonato, clicca su **Open**.

---

## 🔄 4. Il Flusso di Lavoro (Come Collaborare)

Lavorare con Git richiede disciplina per non sovrascrivere il lavoro dei colleghi. Segui **sempre** questo ciclo nell'ordine esatto quando devi fare una modifica:

### Passo 1: Scaricare gli aggiornamenti (PULL)
Prima di iniziare a scrivere, devi assicurarti di avere l'ultima versione. Vai nella scheda **Source Control** (l'icona con i nodi a sinistra) e clicca su **Sync Changes** (o fai *Pull*). Se qualcuno ha aggiunto un paragrafo, lo vedrai comparire.

### Passo 2: Scrivere e Compilare (EDIT)
Apri i file `.tex`, fai le tue modifiche e salva. 
* Per compilare il PDF, clicca sul tasto verde "Play" in alto a destra o usa la combinazione `Ctrl+Alt+V`. Se ci sono errori di sintassi LaTeX, correggili prima di andare avanti.

### Passo 3: Preparare i file (STAGE)
Torna nella scheda **Source Control**. Vedrai l'elenco dei file che hai modificato.
* Clicca sul simbolo **+** accanto ai file `.tex` o alle immagini che hai aggiunto.
* **⚠️ ATTENZIONE:** Non aggiungere *MAI* i file generati dalla compilazione (come `.pdf`, `.log`, `.aux`, `.out`, `.gz`). Il file `.gitignore` dovrebbe già bloccarli in automatico, ma fai sempre attenzione a cosa includi.

### Passo 4: Salvare nella cronologia (COMMIT)
Scrivi un breve messaggio nella casella di testo spiegando cosa hai fatto (es. *"Aggiunta dimostrazione del teorema di Gauss"*) e clicca sul pulsante azzurro **Commit**. Ora la modifica è salvata in modo permanente sul tuo PC.

### Passo 5: Inviare online (PUSH)
Clicca su **Sync Changes**. Questo invierà il tuo salvataggio ai server di GitHub, rendendolo disponibile a tutti i collaboratori.


## Licenza

[![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-sa/4.0/deed.it)

Quest'opera è distribuita con Licenza [Creative Commons Attribuzione - Non commerciale - Condividi allo stesso modo 4.0 Internazionale](https://creativecommons.org/licenses/by-nc-sa/4.0/deed.it).
