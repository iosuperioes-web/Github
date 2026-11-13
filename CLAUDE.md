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

Il rapporto finale va salvato in `rapporti/ronda-AAAA-MM-GG.md`.
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

Su richiesta, prepara in `bozze/` la bozza di un pezzo candidato.

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

---

## Metodo di lavoro con Luca (vale per ogni lavoro, non solo per la ronda)

Disposizione di Luca del 13 novembre 2026. Si applica senza che venga richiesta.

- **Skill che governano:** `argomento-di-massima-potenza` (come si traggono conseguenze dai fatti),
  `stile-santa-maria` (come si scrive), insieme a `protocollo-forense`, `regola-del-negativo`,
  `regola-documento-unico`. Si rileggono a inizio lavoro.
- **Logica:** ogni inferenza ha la sua forma scritta — premessa, legge di copertura, sussunzione,
  alternative, fatto che la rovescerebbe, grado. La logica si tratta come una parte della
  matematica: passaggi espliciti, nessun salto, nessun avverbio al posto di un peso.
- **Retorica:** dialettica pura, diretta al punto in cui l'argomento avversario regge o cede.
  La metafora porta un fatto o una struttura logica; mai ornamento.
- **Storie:** si costruiscono soltanto con i fatti provati nei corpora di evidenza consegnati da Luca,
  ciascuno con la sua fonte.
- **Tono:** umano, essenziale. Niente frasi di riempimento, niente schemi ripetuti.
- **Nessuna autocensura:** si costruisce l'argomento intero; i dubbi stanno a parte, con il loro peso.
  Tagliare è di Luca.
- **Opportunità giuridica:** le valutazioni di opportunità giuridica spettano solo a Luca.
- **Apprendimento:** prima di scrivere a suo nome, si leggono i suoi testi in archivio e se ne
  aggiorna la misura dello stile.
- **Rapporto con la ronda:** il rapporto della ronda è un testo pubblicabile e conserva il registro
  e le regole delle sezioni precedenti (understatement, «in dubbio, escludere»). L'argomento di
  massima potenza è lo strumento di lavoro interno; ciò che esce lo decide Luca.
