# Il Mondo di Ardania

Ardania è il mondo immaginario fantasy del gioco di ruolo di [The Miracle Shard](https://themiraclegdr.com/), un server ("Shard", in gergo) non ufficiale di [Ultima Online](https://en.wikipedia.org/wiki/Ultima_Online) attivo dal 2001.

![The Miracle Shard](banner.jpg)

Il "Background" ruolistico di Ardania (geografia, razze, divinità, bestiario, etc), come descritto nel sito ufficiale (pagina [Background](https://themiraclegdr.com/background/)), è qui raccolto in formato Markdown, per facilitarne l'accesso e l'utilizzo in vari progetti, quali:

- processo e analisi di informazioni tramite strumenti automatici quali AI/LLMs.
- conversione in altri formati (PDF, HTML, audio, etc.)
- conservazione e duplicazione,
- altro...

Grazie a tutto lo [staff](https://themiraclegdr.com/staff/) di The Miracle e a tutti i giocatori!

*Si legge, sbiadita, la seguente firma: "Jack Lake, Hammerheim, 24 Adulain dell'anno Imperiale 289".*

---

## Compilazione in HTML con funzioni di ricerca
È possibile convertire facilmente i files in Markdown in un sito web statico, con funzioni di ricerca, 
utilizzando [jupyter-book](https://jupyterbook.org/en/stable/intro.html), grazie ai due files `_config.yml` e `_toc.yml`.

Il sito, precompilato, è disponibile online: https://jacklake-tm.github.io/ardania-md 

Per crearlo autonomamente, eseguire le seguenti istruzioni (testate su MacOSX):
1. Avere Python 3 installato nel sistema.
2. Clonare il git, creare un virtual environment e scaricare le librerie necessarie:
```
git clone https://github.com/jacklake-tm/ardania-md
cd ardania-md
python3 -m venv .venv
source .venv/bin/activate
pip install jupyter-book
```
3. Eseguire il comando per creare il sito HTML.
```
jupyter-book build .
```
Il risultato sarà disponbile nel folder `/_build/html/`.

## Conversione in PDF

È inoltre possibile produrre un PDF se si ha [Latex](https://en.wikipedia.org/wiki/LaTeX) installato nel sistema, usando il comando:
```
jupyter-book build . --builder pdflatex
```
Il risultato sarà disponbile nel folder `/_build/latex/ardania.pdf`.