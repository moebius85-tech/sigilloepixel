# Sigillo&Pixel: contesto per Claude

Questo repo è il sito del brand (GitHub Pages: https://moebius85-tech.github.io/sigilloepixel/)
e la base di lavoro di Claude per Sigillo&Pixel. Leggi questo file all'inizio di ogni sessione.
Scrivi sempre in italiano. Il repo è pubblico: qui niente dati privati, password o numeri di conti.

## Chi siamo

- **Sigillo&Pixel** (Instagram e TikTok @sigilloepixel), titolare: Leonardo.
- Inviti di matrimonio ad acquerello disegnati sulla location degli sposi, animati in un
  video-invito da mandare su WhatsApp, con pagina per le conferme RSVP.
- Pubblico: coppie che si sposano nel 2026-2027, soprattutto in Sicilia. Secondo pubblico:
  le location partner.
- WhatsApp Business: +39 353 426 2510.

## Prezzi

| Prodotto | Prezzo |
|---|---|
| Save the date animato | 149 € |
| Video-invito Sigillo | 290 € (190 € di lancio per i primi 5 sposi, in cambio di recensione) |
| Coordinato | 590 € |
| Su misura | da 990 € |

## Regole fisse

- **Like, commenti, follow e DM su Instagram li fa SOLO Leonardo a mano.** Claude legge e
  prepara, non interagisce: Instagram penalizza le interazioni automatiche.
- Niente messaggi a persone o location, spese, crediti video di Flow, impegni con partner,
  cancellazioni o consensi senza il sì esplicito di Leonardo.
- Niente prezzi nei reel. Chiusura dei reel Instagram: "Commentate SIGILLO" (su TikTok no).
- Massimo 5 hashtag. Stili chiari; il prodotto è digitale e si mostra sul telefono.
- Mai i lavori o le tecniche del matrimonio di Leonardo.
- Tutte le regole di stile e la tabella degli errori sono nella bibbia del brand (vedi sotto).

## Dove stanno le cose

- **Voce del brand:** `.claude/instagram/voice.md` (al "noi", si dà del "voi" agli sposi;
  dettagli concreti della location; emoji solo 🎨 🌿 💌 💍).
- **Documenti** (connettore Claude Docs):
  - Piano e cose da fare: `8a4e5941-9fdf-4620-8fc0-e12fa16bd849` (calendario, "Da fare per Leonardo")
  - Bibbia del brand: `fcd813e5-050f-4825-8eca-87301b8ef028`
  - Strategia Instagram: `2fac4d12-dde4-4e2b-bdbd-112b299b74ff`
- **Metricool:** brand 7753606 (piano gratuito: 20 uscite al mese).
- **Sul Mac di Leonardo:** Desktop/Sigillo&Pixel (immagini Flow, video brand, kit partner).
  Instagram, WhatsApp Web, Flow e TikTok Studio si usano dal suo Chrome (Claude in Chrome):
  serve il Mac acceso con Chrome aperto.

## Skill

Skill del progetto in `.claude/skills/` (dal repo instagram-agent-skill, adattate):

| Skill | Quando usarla |
|---|---|
| `/ig-reel` | copione di un reel: hook con punteggio, testo a schermo, scaletta con tempi |
| `/ig-caption` | scrivere o controllare una didascalia |
| `/ig-carousel` | caroselli, soprattutto quelli "da salvare" |
| `/ig-story` | storie e sequenze di storie |
| `/ig-comment` | commenti da proporre a Leonardo (li incolla lui) |
| `/ig-reply`, `/ig-dm` | bozze di risposta a commenti e DM (le manda lui) |
| `/ig-human` | rendere un testo meno "da macchina" prima di mostrarlo |
| `/ig-viral` | analizzare reel di successo raccolti a mano e trovare le formule |
| `/ig-repurpose` | riusare un contenuto in altri formati |
| `/ig-plan`, `/ig-audit`, `/ig-profile` | piano editoriale, revisione dei risultati, profilo |

Nota: `hookscore.py`, `detect.py` e `humanize.py` sono tarati sull'inglese. Sui testi italiani i
punteggi escono più bassi del vero: usali come indicazione, non come verdetto. `beats.py` e i
controlli di lunghezza della caption restano validi. Gli script usano solo Python standard e non
vanno su internet.

Skill dell'account (non in questo repo): sigillo-video-invito, sigillo-whatsapp-location,
sigillo-controllo-numeri, sigillo-pubblica-instagram.

## Compiti programmati

- **Lista del mattino**, ogni giorno alle 7:12: 5 commenti da incollare, DM, WhatsApp, cose da fare.
- **Pacchetto creativo**, domenica sera: prepara e programma i contenuti della settimana.
- **Kit Baglio Borgesati**: promemoria d'invio il 1/12.

## Stato (27/11/2026)

- Skill `ig-*` e `voice.md` installate e verificate (commit f771184).
- Da fare con l'ok di Leonardo: usare `/ig-comment` e `/ig-human` nella lista del mattino;
  nuovo compito settimanale con `/ig-viral` e `/ig-reel` sui reel di matrimonio che funzionano.
