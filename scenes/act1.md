# act1

```
SceneSetup.act1();
```

(...300)

n: E QUESTA È LA SUA ANSIA

n: _TU_ SEI L'ANSIA

{{if window.localStorage.continueChapter=="replay"}}
(#act1_replay)
{{/if}}

{{if window.localStorage.continueChapter!="replay"}}
(#act1_normal)
{{/if}}



# act1_replay

`hong({mouth:"0_neutral", eyes:"0_neutral"})`

h: Oh, ciao! Siamo di nuovo qui?

`hong({eyes:"0_neutral"})`

n: IL TUO COMPITO È DI PROTEGGERE L'UMANO DAI *PERICOLI*

`bb({eyes:"look", mouth:"small_lock"})`

n: E INFATTI, RIGIOCARE LO STA RIMETTENDO IN *PERICOLO* PROPRIO ORA

n: PRESTO, AVVISA L'UMANO!

```
sfx("squeak");
bb({body:"squeeze_talk"});
hong({body:"0_squeeze"});
```

b: Ascolta, siamo in pericolo! Chi sta giocando...

[ci torturerà di nuovo!](#act1_replay_torture)

[non troverà un finale alternativo!](#act1_replay_alternate)

[subirà una dissonanza ludonarrativa!](#act1_replay_dissonance)

# act1_replay_torture

```
window.HACK_REPLAY = JSON.parse(localStorage.act4);
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

{{if window.HACK_REPLAY.act1_ending=="fight"}}
b: Ci farà rannicchiare in un angolino a piangere!
{{/if}}

{{if window.HACK_REPLAY.act1_ending=="flight"}}
b: Ci farà spaccare il telefono dopo un attacco di panico!
{{/if}}

{{if window.HACK_REPLAY.a2_ending=="fight"}}
b: *NON* ci farà prendere a pugni chi ha organizzato la festa!
{{/if}}

{{if window.HACK_REPLAY.a2_ending=="flight"}}
b: Ci farà prendere a pugni l'amabile antagonista che ha organizzato la festa!
{{/if}}

{{if window.HACK_REPLAY.a3_ending=="jump"}}
h: Beh, almeno stavolta potremmo non saltare dal te-
{{/if}}

{{if window.HACK_REPLAY.a3_ending=="walkaway"}}
b: CI FARÀ SALTARE DAL TETTO.
{{/if}}

`bb({body:"fear"});`

b: CI ACCADRANNO TUTTE QUESTE NUOVE COSE TERRIBILI, E POI NOI-

(#act1_replay_end)


#act1_replay_alternate

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

h: Certo, la storia nel *complesso* è la stessa, ma ciascun capitolo ha due possibili finali, più le varie opzioni di dialo-

`bb({body:"fear"});`

b: Chi ci gioca si stuferà, chiuderà la scheda del browser, cancellerà il software, e poi noi-

(#act1_replay_end)


# act1_replay_dissonance

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

h: E ora, cosa di così osceno?

`bb({eyes:"normal"});`

b: L'arco narrativo era come poter *SCEGLIERE* di instaurare un rapporto sano con le tue paure,

`bb({eyes:"normal_right"});`

b: Ma tanto rigiocherai la stessa storia, vuol dire che le tue *SCELTE* non contano nulla,

`bb({eyes:"narrow_eyebrow"});`

b: Dimostra una contraddizione tra il messaggio e la meccanica del gioco,

`bb({eyes:"fear"});`

b: E rivela la struttura di questo universo narrativo,

`bb({body:"fear"});`

b: E poi noi-

(#act1_replay_end)


# act1_replay_end

`bb({body:"panic"})`

b: MORIREMOOOOOOOOOOOOOO

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.clearText();
```

(...1001)

```
bb({body:"laugh"});
hong({body:"laugh"});
Game.clearText();
sfx("laugh");
```

(...5001)

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({body:"0_sammich"});
```

h: Ok, torniamo al personaggio.

```
Game.clearText();
```

n4: (LASCIA BLA BLA BLA LA _TUA_ ANSIA BLA BLA BLA CHE PIÙ RAPPRESENTA LE _TUE_ PAURE GIÀ LO SAI)

```
sfx("squeak");
hong({body:"0_squeeze"});
bb({body:"squeeze"});
```

(#act1_normal_choice)



# act1_normal

`hong({mouth:"0_neutral", eyes:"0_annoyed"})`

h: Oh wow, il lupo è tornato. E andiamooo.

`hong({eyes:"0_neutral"})`

n: IL TUO COMPITO È DI PROTEGGERE L'UMANO DAI *PERICOLI*

`bb({eyes:"look", mouth:"small_lock"})`

n: E INFATTI, QUEL PANINO È GIÀ UN *PERICOLO* PROPRIO ORA

n: PRESTO, AVVISA L'UMANO!

```
sfx("squeak");
bb({body:"squeeze_talk"});
hong({body:"0_squeeze"});
```

b: Ascolta, siamo in pericolo! Il pericolo è che...

`bb({body:"squeeze"})`

n4: (LASCIA GIOCARE LA _TUA_ ANSIA! SCEGLI LA RISPOSTA CHE PIÙ RAPPRESENTA LE _TUE_ PAURE)

(#act1_normal_choice)

# act1_normal_choice

[Stiamo pranzando da soli! Di nuovo!](#act1a_alone) `bb({body:"squeeze_talk"})`

[Non stiamo facendo nulla mentre mangiamo!](#act1a_productive) `bb({body:"squeeze_talk"})`

[Il pane bianco fa male!](#act1a_bread) `bb({body:"squeeze_talk"})`

# act1a_alone

```
bb({body:"normal", mouth:"small", eyes:"narrow"});
hong({body:"0_sammich"});
```

b: Lo sapevi che la solitudine cronica è tanto letale quanto fumare 15 sigarette al giorno?

`Game.OVERRIDE_TEXT_SPEED = 2;`

`bb({mouth:"normal", eyes:"normal_right"})`

b: (Holt-Lunstad 2010, PLoS Medicine)

`hong({eyes:"0_annoyed"})`

h: Ehm, grazie per aver citato le fonti, ma-

`Game.OVERRIDE_TEXT_SPEED = 2;`

`bb({body:"fear", mouth:"normal", eyes:"fear"})`

b: Significa che se non usciamo con qualcuno *adesso*, noi-

`bb({body:"panic"})`

b: MORIREMOOOOOOOOOOOOOO

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "alone");
publish("hp_show");
```

(...2500)

`_.fifteencigs = true`

n: HAI USATO *PAURA DI MANCANZA DI AFFETTO*

(#act1b)

# act1a_productive

```
bb({body:"normal", mouth:"small", eyes:"normal"});
hong({body:"0_sammich"});
```

b: Apri il tuo pc e mettiamoci al lavoro, adesso!

`hong({eyes:"0_annoyed"})`

h: Ehm, meglio non lasciare briciole sulla tast-

```
bb({mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Se non contribuiamo al corpo sociale, diventeremo dei parassiti sociali!

b: Il corpo sociale andrà dal dottor Società, che prescriverà dei farmaci che uccide i parassiti sociali e noi-

```
bb({body:"panic", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: MORIREMOOOOOOOOOOOOOO

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "bad");
publish("hp_show");
```

(...2500)

`_.parasite = true`

n: HAI USATO *PAURA DI ESSERE UNA BRUTTA PERSONA*

(#act1b)

# act1a_bread

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich", eyes:"0_annoyed"});
```

h: Quegli studi hanno replicat-

```
bb({body:"fear", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Il grano raffinato alzerà il livello di glicemia, ci dovranno amputare braccia e gambe, e alla fine-

`bb({body:"panic"})`

b: MORIREMOOOOOOOOOOOOOO

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "harm");
publish("hp_show");
```

(...2500)

`_.whitebread = true`

n: HAI USATO *PAURA DI FARSI MALE*

(#act1b)

# act1b

n: È SUPEREFFICACE

`bb({mouth:"smile", eyes:"smile"});`

b: Capito? Sono il tuo fedele lupo da guardia!

`bb({body:"pride_talk"});`

b: Segui tuo istinto! Le tue emozioni sono valide!

`bb({body:"pride"});`

n: PORTA A ZERO LA BARRA DELL'ENERGIA UMANA

n: PER PROTEGGERE I SUOI BISOGNI FISICI + SOCIALI + MORALI, USA:

n: PAURA DI *FARSI MALE* #harm#

n: PAURA DI *MANCANZA DI AFFETTO* #alone#

n: E PAURA DI *ESSERE UNA BRUTTA PERSONA* #bad#

`Game.OVERRIDE_TEXT_SPEED = 1.25;`

n4: (CONSIGLIO: FAI LE SCELTE CHE PIÙ COLPISCONO LE TUE PAURE INTERIORI!~)

h: ...

```
hong({body:"putaway"});
sfx("rustle");
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

(...1000)

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

h: Sai che c'è? Forse mi metto un po' al telefono.

```
sfx("rustle2");
hong({body:"phone1", mouth:"neutral", eyes:"neutral"})
```

n: PROTEGGI L'UMANO

n: DAL MONDO. DAGLI ALTRI. DA SÉ STESSO.

n: IN BOCCA AL LUPO

(...500)

`Game.clearText()`

(...500)

(#act1c)

# act1c

`music('battle', {volume:0.5})`

n: ROUND ONE: *FIGHT!*

`bb({body:"normal", mouth:"normal", eyes:"normal"});`

h: Uh, su Facebook c'è scritto che ci sarà una festa questo weekend.

`bb({eyes:"uncertain"});`

b: Ma quel fenomeno organizza una festa *tutti* i weekend?

`bb({eyes:"uncertain_right"});`

b: Che vuoto interiore sta cercando di colmare? Dev'essere proprio fuori di testa!

`hong({eyes:"surprise"});`

h: E ho persino ricevuto un invito?

`bb({eyes:"fear", mouth:"normal"});`

b: Che bello!

[Conferma, o moriremo di solitudine!](#act1c_loner)

[Rifiuta, è pieno di droghe pericolose!](#act1c_drugs)

[Ignora, noi siamo dei guastafeste.](#act1c_sad)

# act1c_loner

{{if _.fifteencigs}}
b: Quindici sigarette al giorno, umano! Quindici!
{{/if}}

{{if !_.fifteencigs}}
`Game.OVERRIDE_TEXT_SPEED = 1.5;`
{{/if}}

{{if !_.fifteencigs}}
b: E poi nessuno verrà al nostro funerale, butteranno le nostre ceneri all'oceano, verremo mangiati da una balena,
{{/if}}

{{if !_.fifteencigs}}
b: e diventeremo CACCA DI BALENA!
{{/if}}

{{if !_.fifteencigs}} `_.whalepoop = true` {{/if}}

(...500)

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`bb({eyes:"normal"});`

{{if !_.fifteencigs}}
b: Quindi sì, dovremmo andare a quella festa!
{{/if}}

{{if _.parasite}}
b: Porta il pc, così potremo lavorare e non essere dei parassiti-società
{{/if}}

{{if _.whitebread}}
b: Basta che non servono PANE BIANCO
{{/if}}

`hong({mouth:"anger", eyes:"anger"});`

h: ODDIO. Se questo ti farà chiudere il becco, va bene.

h: Accetto l'invito.

{{if _.whalepoop}}
b: Cacca di balena, umano! Cacca di balena!
{{/if}}

`_.partyinvite="yes"`

(#act1d)

# act1c_drugs

`bb({mouth:"small", eyes:"fear"});`

{{if _.whitebread}}
b: o ancora peggio... PANE BIANCO
{{/if}}

{{if _.whitebread}}
`Game.OVERRIDE_TEXT_SPEED = 1.5;`
{{/if}}

{{if _.whitebread}}
b: Faremo overdose di metanfetamina e pane bianco tanto che non riusciranno a mettere il nostro cadavere grasso nel forno crematorio!
{{/if}}

{{if !_.whitebread}}
b: Faremo overdose di talmente tante droghe che il becchino si chiederà come il nostro corpo sia *già* stato imbalsamato!
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

{{if _.parasite}}
b: Per di più, non possiamo fare festa, dobbiamo lavorare, o diventeremo degli orribili parassiti-società!
{{/if}}

`hong({mouth:"anger", eyes:"anger"});`

h: ODDIO. Se questo ti farà chiudere il becco, va bene.

h: Rifiuto l'invito.

`_.partyinvite="no"`

(#act1d)

# act1c_sad

`bb({eyes:"uncertain_right", mouth:"normal"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

{{if _.fifteencigs}}
b: Tuttò ciò che facciamo è stare in un angolino a piangere su come la solitudine sia mortale quanto fumare 15 sigarette al giorno.
{{/if}}

{{if _.parasite}}
b: Tutto ciò che facciamo alle feste è preoccuparci di come invece potremmo essere produttivi.
{{/if}}

{{if _.whitebread}}
b: Tutto ciò che facciamo è preoccuparci di come i cibi spazzatura ci uccideranno.
{{/if}}

```
bb({mouth:"normal", eyes:"normal"});
hong({mouth:"neutral", eyes:"lookaway"});
```

h: Cavolo, mi chiedo il perché.

`hong({eyes:"neutral"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

b: Quindi, se ci andiamo, li faremo sentire in colpa, ma anche se non andiamo li faremo sentire in colpa!

`bb({body:"fear", eyes:"fear"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

b: TUTTO CIÒ CHE FACCIAMO E FAR SENTIRE IN COLPA LE PERSONE, NOI DOVREMMO SENTIRCI IN COLPA

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

`hong({mouth:"anger", eyes:"anger"});`

h: Uff. Se questo ti farà chiudere il becco, va bene.

h: Ignoro l'invito.

`_.partyinvite="ignore"`

(#act1d)

# act1d

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"neutral", eyes:"annoyed"});
```

h: Comunque. Basta Facebook. Mi serve qualcosa di più tranquillo, che non mi faccia venire ansia.

`hong({eyes:"neutral"});`

h: Che succede su Twitter?

`bb({eyes:"look"});`

[Oh no, leggi questa terribile notizia!](#act1d_news)

[Oh no, quel tweet parla di nascosto di *noi?*](#act1d_subtweet)

[Uh, una GIF di un gatto che beve il latte](#act1d_milk)


# act1d_news

```
bb({eyes:"pained1"});
music(null, {fade:2});
```

b: Cavolo, è come se il mondo stesse andando a fuoco, vero?

```
bb({eyes:"pained2"});
hong({mouth:"sad", eyes:"sad"});
```

b: Come se tutto stesse finendo e morendo, siamo condannati, e non c'è nulla che possiamo fare.

```
Game.OVERRIDE_TEXT_SPEED = 0.5;
bb({mouth:"shut"});
```

b: ...

`bb({mouth:"smile", eyes:"smile"});`

b: Retwitta la storia!

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

`_.badnews=true`

```
music('battle', {volume:0.5});
hong({mouth:"anger", eyes:"anger"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Ok, la retwitto, basta che fai silenzio!

`hong({mouth:"neutral", eyes:"annoyed"});`

h: Al diavolo, andiamo su Snapchat.

(#act1e)


# act1d_subtweet

`bb({eyes:"fear"});`

b: È una frecciatina! Una vile, subdola feecciatina!

`hong({eyes:"annoyed"});`

h: Magari no?

`bb({eyes:"narrow", mouth:"small"});`

b: E se ci stessero sparlando alle spalle?

h: Non ci-

`bb({body:"fear", eyes:"fear", mouth:"normal"});`

b: ALLE NOSTRE SPALLE

`hong({eyes:"sad", mouth:"sad"});`

h: Io-

`bb({eyes:"narrow", mouth:"small"});`

b: *E se*

h: S-

`bb({eyes:"narrow_eyebrow"});`

b: *E se*

```
Game.OVERRIDE_TEXT_SPEED = 0.5;
hong({mouth:"shut"});
```

h: ...

(...1000)

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`_.subtweet=true`

```
hong({mouth:"anger", eyes:"annoyed"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: O-ok, andiamo su Snapchat.

(#act1e)

# act1d_milk

`hong({mouth:"smile", eyes:"neutral"});`

h: Eheh, che carino, retwittiamolo, pens-

```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b: I GATTI NON DIGERISCONO IL LATTE, E NOI SIAMO DELLE PERSONE ORRIBILI A GUSTARCI L'ABUSO SUGLI ANIMALI

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
attack("18p", "bad");
```

(...2500)


`_.catmilk=true`

```
hong({mouth:"anger", eyes:"annoyed"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: O-ok, andiamo su Snapchat.

(#act1e)

# act1e

`hong({mouth:"neutral", eyes:"neutral"});`

h: Uh, le foto di ieri sera. Allora è *così* che son fatte quelle feste settimanali.

{{if _.partyinvite=="yes"}} (#act1e_said_yes) {{/if}}

{{if _.partyinvite=="no"}} (#act1e_said_no) {{/if}}

{{if _.partyinvite=="ignore"}} (#act1e_said_ignore) {{/if}}

# act1e_said_yes

`hong({mouth:"sad", eyes:"annoyed"});`

h: Uff, sembra troppo affollato per la mia ansia.

h: Forse non avrei dovuto accettare?

```
hong({mouth:"neutral", eyes:"neutral"});
bb({mouth:"normal", eyes:"normal"});
```

[Cambi risposta? Come un idiota?!](#act1e_yes_dontchange)

[Cambia risposta! Troppo affollato!](#act1e_yes_changetono)

{{if _.subtweet}}
[Sì, ci stavano decisamente lanciando una frecciatina.](#act1e_ignore_subtweet)
{{/if}}

{{if _.badnews}}
[Aspetta, abbiamo retwittato senza verificare i fatti.](#act1e_ignore_factcheck)
{{/if}}

{{if (!_.subtweet && !_.badnews)}}
[Sai che hai davvero un pessimo atteggiamento?](#act1e_ignore_posture)
{{/if}}

# act1e_yes_dontchange

```
bb({eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Contavano sulla nostra presenza e ora stiamo tradendo la loro fiducia? Vuoi morire così, senza nessuno?!

{{if _.fifteencigs}}
b: QUINDICI. SIGARETTE.
{{/if}}

{{if _.whalepoop}}
b: CACCA. DI. BALENA.
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

```
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Va bene, smettila, lascerò la conferma!

(#act1f)

# act1e_yes_changetono

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Non sai nulla sulle fughe precipitose?

```
bb({body:"fear", mouth:"small", eyes:"narrow"});
hong({eyes:"sad", mouth:"sad"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Nel 2003, nel Rhode Island, ci fu un incendio in una discoteca, col panico si creò un ingorgo alle uscite, causando la morte di 100 persone-

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({mouth:"shock"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: VUOI CHE SUCCEDA A NOI-

```
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 2.5;
```

b: METTI NO METTI NO METTI NO METTI NO METTI NO METTI NO METTI NO METTI NO METT-


```
bb({body:"normal", eyes:"fear", mouth:"normal"});
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

```
hong({eyes:"anger", mouth:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Va bene, smettila, cambio risposta in "no"! Santo cielo!

(#act1f)

# act1e_said_no

`hong({mouth:"sad", eyes:"sad"});`

h: Uhm... sembra divertente.

h: Forse non avrei dovuto rifiutare?

`bb({mouth:"normal", eyes:"normal"});`

[Cambi risposta? Come un idiota?!](#act1e_no_dontchange)

[Cambia risposta! Non morire senza nessuno!](#act1e_no_changetoyes)

{{if _.subtweet}}
[Sì, ci stavano decisamente lanciando una frecciatina.](#act1e_ignore_subtweet)
{{/if}}

{{if _.badnews}}
[Aspetta, abbiamo retwittato senza verificare i fatti.](#act1e_ignore_factcheck)
{{/if}}

{{if (!_.subtweet && !_.badnews)}}
[Sai che hai davvero un pessimo atteggiamento?](#act1e_ignore_posture)
{{/if}}

# act1e_no_dontchange

`bb({eyes:"anger"})`

b: Tutti contavano sul fatto che...

b: Li lasciassimo festeggiare spensierati senza un orribile e disgustoso verme {{if _.whitebread}}mangia-pane-bianco{{/if}} come te-


```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

```
bb({body:"normal", eyes:"uncertain", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Va bene, smettila, lascio così!

(#act1f)

# act1e_no_changetoyes

```
bb({body:"fear", eyes:"fear", mouth:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: La solitudine cronica alza i livelli di cortisolo e aumenta i rischi di infarto e malattie cardiovascolari!

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

{{if _.fifteencigs}}
b: QUINDICI. SIGARETTE.
{{/if}}

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Va bene, smettila, cambio risposta in "sì"! Santo cielo!

(#act1f)

# act1e_ignore_subtweet

```
bb({eyes:"fear", mouth:"small"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Tutti i nostri tweet problematici sono ritornati a galla!

```
bb({body:"fear", eyes:"fear", mouth:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.7;
```

b: Verremo richiamati, sospesi, e portati via verso l'autostrada delle informazioni con una corda attaccata alla sella di un cavallo!

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Perché sei così?!

(#act1f)

# act1e_ignore_factcheck

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Stiamo diffondendo disinformazione! Stiamo minando la fiducia nella libertà di stampa!

```
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Per colpa nostra, il fascismo emergerà dalle macerie della democrazia!

```
bb({body:"normal", eyes:"anger"});
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

```
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
_.factcheck = true;
```

h: Perché sei così?!

(#act1f)

# act1e_ignore_posture

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Vuoi avere un pretzel al posto della spina dorsale?! Smettila di ingobbirti davanti allo schermo!

```
bb({body:"meta"});
```

b: Lo stesso vale per te.

```
bb({body:"normal", mouth:"normal"});
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Perché sei così?!

(#act1f)

# act1e_said_ignore

`hong({mouth:"sad", eyes:"sad"});`

h: Uhm... sembra divertente.

h: Forse non avrei dovuto rifiutare l'invito?

`bb({mouth:"normal", eyes:"normal"});`

[Continua ad ignorare, siamo sempre dei guastafeste.](#act1e_ignore_continue)

[Non ignorare e accetta.](#act1e_ignore_changetoyes)

[Non ignorare e rifiuta.](#act1e_ignore_changetono)

# act1e_ignore_continue

`hong({eyes:"annoyed"});`

h: Però non è molto carino continuare ad ignorare, giusto?

`bb({eyes:"normal_right"});`

b: Beh, gli altri *ci* ignorano sempre, perciò...

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`bb({eyes:"normal"});`

b: Immagino siamo pari.

(#act1f)

# act1e_ignore_changetoyes

`hong({eyes:"surprise", mouth:"smile"});`

h: Tu... lasceresti che mi diverta?

b: Beh, sai com'è, stare soli *può* ucciderci.

`hong({eyes:"neutral", mouth:"neutral"});`

(#act1e_no_changetoyes)

# act1e_ignore_changetono

`bb({eyes:"narrow"});`

b: Troppo affollato. Le folle sono pericolose.

(#act1e_yes_changetono)


# act1f

```
hong({mouth:"neutral", eyes:"neutral"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: Va beh. Oh, una notifica su Tinder.

`bb({eyes:"uncertain"})`

b: Cosa, l'app di incontri?

`hong({eyes:"annoyed"})`

h: Non è un'app di incontri, è solo un modo per conoscere pers-

`bb({eyes:"narrow"})`

b: È un'app di incontri.

```
hong({eyes:"surprise", mouth:"smile"});
bb({eyes:"normal"});
```

h: Oh, un match! Non sembra male!

```
bb({eyes:"narrow_eyebrow"});
hong({eyes:"sad", mouth:"anger"})
```

h: Ti prego, non mi rovinare quest-

```
bb({body:"panic"});
Game.OVERRIDE_TEXT_SPEED = 2.0;
```

b: ALLARME ALLARME ALLARME ALLARME ALLARME ALLARME

`bb({body:"fear", eyes:"fear", mouth:"normal"})`

[Siamo *sfruttati* dagli altri.](#act1f_used_by_others)

[Stiamo *sfruttando* gli altri.](#act1f_using_others)

[IL TUO MATCH È UN SERIAL KILLER](#act1f_killer)

# act1f_used_by_others

`bb({body:"point_crotch", eyes:"normal", mouth:"normal"})`

b: Gli incontri casuali potrebbero colmare il vuoto laggiù,

b: ma non potranno mai colmare il vuoto...

`bb({body:"point_heart", eyes:"pretty", mouth:"small"})`

b: Qua *dentro*.

(...1000)

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Il punto è che MORIREMO DA SOLI

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`_.hookuphole=true`

(#act1g)

# act1f_using_others

`bb({eyes:"narrow", mouth:"small"})`

b: Pensi che i genitali delle persone siano come dei Pokémon da collezionare?

```
bb({body:"sing", eyes:"pretty", mouth:"shut"});
music("pokemon");
Game.clearText();
Game.FORCE_CANT_SKIP = true;
```

```
Game.FORCE_TEXT_DURATION = 1000;
Game.FORCE_NO_VOICE = true;
```

b: ♫ (sigla Pokémon)-

(...5600)

```
bb({mouth:"normal"});
Game.FORCE_TEXT_DURATION = 2400;
```

b: ♫ Girovagando per il mondo-

(...500)

```
bb({eyes:"narrow", mouth:"small"});
Game.FORCE_TEXT_DURATION = 2100;
```

b: ♫ Il mio uccello lancerò-

(...1500)

```
bb({eyes:"pretty"});
Game.FORCE_TEXT_DURATION = 2300;
```

b: ♫ Ed ogni Porke-mon-

(...500)

```
bb({eyes:"fear", mouth:"normal"});
Game.FORCE_TEXT_DURATION = 2000;
```

b: ♫ Così io ^scoperò^! WOOOH!

(...1000)

```
bb({eyes:"smile", mouth:"smile"});
Game.FORCE_TEXT_DURATION = 1000;
```

b: ♫ VIVA I PORKE-MON! ^TETTE^ PROROMP-

```
Game.FORCE_CANT_SKIP = false;
Game.clearText();
music(false);
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Il punto è che siamo dei vermi manipolatori.

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

`_.pokemon=true`

(#act1g)

# act1f_killer

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

{{if _.whitebread}}
b: Ti intrappolerà in un pozzo e ti farà mangiare a forza pane bianco, così ingrassi e poi con la tua pelle ci farà un vestito!
{{/if}}

{{if _.parasite}}
b: Ti picchierà con un timer pomodoro, urlando "NON STAI FACENDO NULLA, PARASSITA"
{{/if}}

{{if !_.whitebread && !_.parasite}}
b: Ti strapperà la carne riducendola in coriandoli di sangue, trasformerà le tue viscere in stelle filanti, e mescoleranno il tuo sangue nel ciotolne del punch!
{{/if}}

{{if !_.whitebread && !_.parasite}}
b: QUESTO mi sembra un ottimo invito, no?!
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

`_.serialkiller=true`

(#act1g)

# act1g

```
bb({body:"normal", mouth:"normal", eyes:"look"});
hong({body:"2_tired"});
Game.OVERRIDE_TEXT_SPEED = 0.5;
music(false);
```

h: ...

(...500)

h: Questo gioco mi ha stufato.

(...700)

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

h:
{{if _.fifteencigs}}"la solitudine ci ucciderà"... {{/if}}
{{if _.parasite}}"siamo dei parassiti-società"... {{/if}}
{{if _.whitebread}}"non mangiarlo, ci ucciderà"... {{/if}}
{{if _.subtweet}}"ci sparlano alle spalle"... {{/if}}
{{if _.badnews}}"il mondo sta andando a fuoco"... {{/if}}
{{if _.hookuphole}}"moriremo soli"... {{/if}}
{{if _.serialkiller}}"è un serial killer"... {{/if}}
{{if _.catmilk}}"i gatti non digeriscono il latte"... {{/if}}
{{if _.pokemon}}una schifosa parodia di una canzone... {{/if}}

h: Voglio solo vivere la mia vita.

h: Voglio solo liberarmi da questo... dolore.

`bb({eyes:"look_sad"});`

b: Ehi... umano...

`Game.OVERRIDE_TEXT_SPEED = 0.5;`

b: Andrà tutto bene.

(...600)

`bb({body:"point_heart", eyes:"look_sad_smile", mouth:"smile"});`

b: In quanto tuo lupo da guardia, farò sempre attenzione ai pericoli, e farò del mio meglio per tenerti al sicuro.

`bb({body:"normal", eyes:"look_sad", mouth:"smile"});`

b: Promesso.

(...600)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({body:"phone1", eyes:"neutral", mouth:"neutral"});
```

h: Ultima app. Instagram: cos'hai per me?

`hong({eyes:"sad"});`

h: Altre... foto di feste.

`hong({mouth:"sad"});`

h: Sembrano tutti così felici. Liberi dalle preoccupazioni. Dalle ansie.

`hong({mouth:"anger"});`

h: Dio, perché non posso essere come loro? Perché non posso essere *normale?*

`bb({eyes:"normal_right"});`

b: A proposito di feste, riguardo all'invito di questo weekend. Ecco la mia risposta DEFINITIVA:

`bb({eyes:"normal"});`

[Dovremmo andare.](#act1g_go) `Game.OVERRIDE_CHOICE_LINE=true`

[Non dovremmo andare.](#act1g_dont) `Game.OVERRIDE_CHOICE_LINE=true`

# act1g_go

`_.act1g = "go"`

(#act1h)

# act1g_dont

`_.act1g = "dont"`

(#act1h)

# act1h

b: Dovremm-

```
bb({eyes:"wat", mouth:"small"});
hong({body:"2_fuck"});
```

h: VAI A

`hong({body:"2_you"});`

h: FARTI *^FOTTERE^*

(...500)

b: c-

(...1500)

`bb({eyes:"wat_2"});`

b: cos?

`hong({body:"phone1", eyes:"anger", mouth:"anger"});`

h: Dirò di SÌ a quella festa,

{{if _.act1g=="go"}}
h: e NON perché tu vuoi che ci vada, ma perché *io* voglio.
{{/if}}

{{if _.act1g=="dont"}}
h: Anzi, PERCHÉ non vuoi che ci vada.
{{/if}}

```
hong({body:"putaway"});
sfx("rustle");
```

h: Tu NON hai il controllo della mia vita.

```
sfx("rustle2");
hong({body:"0_sammich", eyes:"0_annoyed", mouth:"0_neutral"});
```

h: E ora, scusami, vado a mangiare questo delizioso panino in santa pace.
`hong({body:"2_sammich_eat"});`

(...601)

```
sfx("sandwich");
hong({body:"2_sammich_eaten", eyes:"0_lookaway", mouth:"0_chew1"})
```

(...601)

```
bb({body:"normal", eyes:"uncertain", mouth:"shut"});
Game.OVERRIDE_TEXT_SPEED = 0.5;
```

b: ...

```
bb({eyes:"normal_right"});
Game.OVERRIDE_TEXT_SPEED = 1;
```

b: ...

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 4;
```

b: ..................

(...500)

`bb({mouth:"normal"});`

[AHHHH MORIREMO](#act1h_death) `Game.OVERRIDE_CHOICE_LINE = true;`

[AHHHH CI ODIANO TUTTI](#act1h_loneliness) `Game.OVERRIDE_CHOICE_LINE = true;`

[AHHHH SIAMO DELLE PERSONE ORRIBILI](#act1h_worthless) `Game.OVERRIDE_CHOICE_LINE = true;`

# act1h_death

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: AHHHH MORIREMO AAAAAAHHHHHHH

```
hong({body:"3_defeated1"});
attack("100p", "harm");
```

(...2500)

(#act1i)

# act1h_loneliness

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: AHHHH CI ODIANO TUTTI AAAAAAHHHHHHH

```
hong({body:"3_defeated1"});
attack("100p", "alone");
```

(...2500)

(#act1i)

# act1h_worthless

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: AHHHH SIAMO DELLE PERSONE ORRIBILI AAAAAAHHHHHHH

```
hong({body:"3_defeated1"});
attack("100p", "bad");
```

(...2500)

(#act1i)

# act1i

```
bb({mouth:"smile_lock", eyes:"smile", body:"normal"});
music('battle', {volume:0.5});
```

n: CONGRATULAZIONI

(...500)

n: HAI PROTETTO I BISOGNI FISICI + SOCIALI + MORALI DELL'UMANO CON SUCCESSO

n: PERCHÉ? GUARDA COM'È RICONOSCENTE!

(...500)

n: ORA CHE LA SUA ENERGIA È A ZERO, PUOI DIRETTAMENTE CONTROLLARE LE SUE AZIONI

`bb({mouth:"smile", eyes:"normal"});`

n: SCEGLI LA TUA MOSSA FINALE

`bb({mouth:"small_lock", eyes:"fear"});`

n: *DAI IL COLPO DI GRAZIA*

[{LOTTA: Dai una punizione al tuo telefono straziante!}](#act1i_phone) `Game.OVERRIDE_CHOICE_LINE=true`

[{LOTTA: Rannicchiati in un angolino a piangere!}](#act1i_cry) `Game.OVERRIDE_CHOICE_LINE=true`

# act1i_phone

`bb({mouth:"normal", eyes:"narrow"})`

b: Il tuo telefono ti stava facendo venire un attacco di panico!

`bb({eyes:"anger"})`

b: Zuckerberg e compagnia bella stanno sabotando la tua salute mentale e fare soldi per gli investitori!

```
bb({body:"fear", eyes:"fear"});
hong({body:"3_defeated2"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Punisci il telefono! Distruggilo! Uccidilo!

```
Game.OVERRIDE_TEXT_SPEED = 2.5;
bb({body:"flail"});
hong({body:"3_defeated3"});
_.act1_ending = "fight";
```

b: UCCIDI UCCIDI UCCIDI UCCIDI UCCIDI UCCIDI UCCIDI UCCIDI UCCIDI UCCIDI UCCIDI UCCIDI UCCIDI UCCIDI UCCIDI UCCID--

(#act1j)

# act1i_cry

`bb({eyes:"fear", mouth:"normal"})`

b: Il mondo intero è pieno di pericoli!

```
bb({body:"fear"});
hong({body:"3_defeated2"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Fai come gli armadilli! Rannicchiati in segno di auto-difesa!

```
Game.OVERRIDE_TEXT_SPEED = 2.5;
bb({body:"flail"});
hong({body:"3_defeated3"});
_.act1_ending = "flight";
```

b: RANNICCHIATI E PIANGI RANNICCHIATI E PIANGI RANNICCHIATI E PIANGI RANNICCHIATI E PIANGI RANNICCH-- 

(#act1j)

# act1j

`SceneSetup.act1_outro()`
