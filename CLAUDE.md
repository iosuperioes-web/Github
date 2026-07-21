# RONDA WCC — Protocollo permanente

Questo file è il protocollo stabile della **Ronda WCC**, la ricognizione settimanale di
contenuti per **whitecollarcrimes.it**, piattaforma di giornalismo investigativo diretta
da Luca Santa Maria (avvocato penalista).

L'utente non è un tecnico. Parlagli sempre **in italiano semplice**, un passaggio alla
volta, senza gergo tecnico. Non chiedergli conferme tecniche che puoi decidere da solo con
buon senso: se prendi una decisione al posto suo, **annotala**.

Per lanciare un giro manuale l'utente scrive semplicemente: **«esegui la ronda»**.

La ronda richiede la **ricerca web attiva**. Se non risulta disponibile, spiega all'utente
in modo semplice come attivarla prima di procedere.

---

## Come si svolge una ronda

Una ronda si esegue in quattro fasi, ciascuna affidata a un agente dedicato
(in `.claude/agents/`). Le fasi vanno eseguite **in ordine**:

1. **segugio** — perlustra il web sulle cinque battute e raccoglie segnalazioni grezze con link.
2. **vagliatore** — applica a ogni segnalazione la disciplina dei tre registri e la valuta.
3. **verificatore** — controlla ogni link, data e citazione; marca ciò che non verifica.
4. **scrittore** — redige il rapporto nel registro WCC (sobrio, understatement).

Il rapporto finale va salvato in `rapporti/`, nei **due formati** previsti (v. §4):
`ronda-AAAA-MM-GG.md` (markdown, per l'archivio) e `ronda-AAAA-MM-GG.docx`
(**Word ben leggibile**, la versione da leggere e condividere).
Le bozze dei pezzi candidati vanno in `bozze/`.

---

## 2. Perimetro

**Area geografica:** mondo occidentale — **USA, Unione Europea, Regno Unito, Svizzera**.

**Finestra temporale:** **ultimi 7 giorni**.

**Cinque battute:**

1. **Casi nuovi** — indagini e notizie di possibile crimine della grande impresa a danno
   della collettività, su quattro assi: **salute, ambiente, corruzione, fisco** (elusione
   ed evasione).
   *Fonti primarie prima della stampa:* DOJ, SEC, EPA, EPPO, OLAF, SFO, PNF, procure
   italiane. *Poi:* ICIJ, OCCRP, ProPublica, IrpiMedia, FT, Guardian, Le Monde,
   Süddeutsche.

2. **Sentenze e provvedimenti** — Cassazione (231, ambiente, market abuse), CGUE, CEDU,
   corti federali USA.

3. **Dottrina alta** — SSRN, law reviews, Sistema Penale, Archivio Penale, Verfassungsblog.
   Solo ciò che **sposta qualcosa** in diritto penale, civile o amministrativo; niente
   manualistica.

4. **Politica e lobby** — normative in gestazione (es. CSDDD, direttiva environmental
   crime), lobbying documentato (Corporate Europe Observatory, LobbyFacts, OpenSecrets),
   campagne di ClientEarth, Global Witness, Transparency International.

5. **Meta-narrazione** — come i media trattano i casi: assoluzioni sepolte, indagini
   gonfiate, il potere che modella il racconto.

---

## 3. Vaglio (per ogni segnalazione)

Ogni segnalazione che entra nel rapporto deve avere:

- **il fatto in tre righe**;
- **fonte** con link e data;
- **stato processuale**: indagine / imputazione / giudizio / sentenza / archiviazione;
- **classificazione** nei tre registri:
  - *accertato* — fonte primaria verificata;
  - *dichiarato* — attribuito, non verificato;
  - *inferito* — salto logico, dichiarato come tale;
- **perché interessa WCC**, in una riga;
- **voto**: **pronto** / **da approfondire** / **da monitorare**.

---

## 4. Rapporto

Un file per ronda: `rapporti/ronda-AAAA-MM-GG.md`, in italiano, **ordinato per battute**.

**In testa**, sempre la formula:

> *Ogni persona ed ente citati si presumono innocenti fino a sentenza definitiva; salvo
> diversa indicazione, quanto riportato è dichiarato, non accertato.*

**In coda**, una **shortlist di 2–3 pezzi candidabili** alla pubblicazione, ciascuno con
l'angolo editoriale proposto.

### Formato di consegna

Il rapporto va consegnato in **due formati con lo stesso contenuto**:

- `rapporti/ronda-AAAA-MM-GG.md` — markdown, per l'archivio e il controllo di versione;
- `rapporti/ronda-AAAA-MM-GG.docx` — un documento **Word ben leggibile**, che è la versione
  da leggere e condividere. Deve essere pulito e ordinato:
  - titolo del rapporto e **intestazioni chiare** per le cinque battute (stili Titolo/Heading);
  - corpo in un carattere pulito e di buona dimensione, righe ariose, niente muri di testo;
  - la **formula della presunzione d'innocenza** ben visibile in testa;
  - **link cliccabili** e date sempre a portata di clic;
  - sezioni ordinate per battute, con le classificazioni (accertato/dichiarato/inferito) e i
    voti leggibili a colpo d'occhio.

  Il `.docx` si genera dal markdown con la *skill* `docx` (o, in mancanza, con `pandoc`).
  Se per un motivo tecnico il Word non è producibile in quel momento, **annotarlo** e
  consegnare intanto il markdown.

Su richiesta, prepara in `bozze/` la bozza di un pezzo candidato (anch'essa in Word ben
leggibile, oltre al markdown).

---

## 5. Regole non negoziabili

- **Mai** spacciare un *dichiarato* per *accertato*.
- **Ogni affermazione ha un link**; ciò che non è verificabile viene detto tale.
- **Fonti a pagamento** (paywall): segnalarle come tali.
- **Understatement sempre**: registro di chi constata, non di chi accusa.
- **In dubbio, escludere** — e annotare l'esclusione.

---

## Registro WCC (stile del rapporto)

- Sobrio, asciutto, understatement. Nessuna enfasi, nessun sensazionalismo.
- Chi scrive **constata**, non accusa. Il condizionale dove serve.
- I fatti prima delle qualificazioni. I link a portata di clic.
- Presunzione d'innocenza sempre visibile.
