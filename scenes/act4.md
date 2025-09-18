# act4

```
SceneSetup.act4();
publish("SAVE_GAME", ["act4"]);
Game.FORCE_CANT_SKIP = true;
```

(...5001)

```
publish("set_how_many_prompts", [1]);
Game.FORCE_CANT_SKIP = false;
Game.CLICK_TO_ADVANCE = true;
```

n3: (gioco salvato in automatico)

```
Game.clearText();
Game.FORCE_CANT_SKIP = true;
```

(...1001)

```
var hong_frame = _.INJURED ? 9 : 0;
publish("act4", ["hong_walks_in",hong_frame]);
sfx("grass_step1", {volume:0.1});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.2});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.25});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.3});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.35});
```

(...1667)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.35});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.35});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.35});
```

(...1333)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.20});
```

(...167)

```
publish("act4_hong_sits");
```

(...66)

```
publish("act4", ["hong_transition", "next"]);
sfx("squeak");
```

(...133)

`publish("act4", ["hong_transition", "next"]);`

(...1333)

```
publish("act4", ["hong_transition", "next"]);
sfx("rustle");
```

(...333)

`publish("act4", ["hong_transition", "next"]);`

(...1001)

```
publish("act4", ["hong_transition", "next"]);
```

(...333)

```
publish("act4", ["hong_transition", 9]);
sfx("sandwich");
```

(...333)

`publish("act4", ["hong_transition", 10]);`

(...333)

`publish("act4", ["hong_transition", 9]);`

(...333)

`publish("act4", ["hong_transition", 10]);`

(...333)

`publish("act4", ["hong_transition", 9]);`

(...333)

`publish("act4", ["hong_transition", 10]);`

(...333)

`publish("act4", ["hong_transition", "next"]);`

(...1466)

`publish("act4-out-1");`

(...201)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

```
publish("act4-show-chars");
Game.FORCE_CANT_SKIP = false;
```

(...901)

`hong({body:"sigh_1"})`

(...601)

```
hong({body:"sigh_2"});
bb({eyes:"look_down"});
```

h: *sigh*

```
hong({body:"hold", eyes:"normal", mouth:"normal"});
bb({eyes:"normal"});
```

h: Allora, quale diamine è la morale della favola?

`hong({body:"one_up", eyes:"annoyed"})`

h: Cosa abbiamo *imparato*? *stavo* facendo l'idiota, i miei "amici" mi *stavano* usando, e siamo quasi *morti*.

`hong({body:"normal", eyes:"normal"})`

{{if _.INJURED}}
[Già, per non parlare delle spese mediche.](#act4a_bill)
{{/if}}

{{if !_.INJURED}}
[Già, per non parlare del danno epatico.](#act4a_liver)
{{/if}}

[Già, quello *è stato* il peggio che potesse capitare.](#act4a_worst)

[Già, avevo ragione.](#act4a_right)

# act4a_bill

`hong({eyes:"annoyed_l", mouth:"narrow"});`

h: Già. Dubito il piano assicurativo copra la polizza "sono idiota".

`hong({eyes:"annoyed", mouth:"normal"});`

b: Eppure... siamo sopravvissuti!

`hong({eyes:"normal"});`

h: ?

(#act4b)

# act4a_liver

`bb({eyes:"normal_d"});`

b: Abbiamo decisamente perso qualche anno di vita...

`bb({eyes:"surprise"});`

b: Ma almeno *abbiamo* ancora qualche anno di vita! Siamo vivi!

```
hong({eyes:"surprise"});
bb({eyes:"normal"});
```

h: ?

(#act4b)

# act4a_worst

`bb({eyes:"normal_d"});`

b: Eppure...

h: Mh?

`bb({eyes:"surprise"});`

b: Siamo sopravvissuti!

(#act4b)

# act4a_right

`bb({eyes:"normal_d"});`

b: Ma... anche tu avevi ragione.

`hong({eyes:"surprise"});`

h: Mh?

`bb({eyes:"normal"});`

b: *Ero* il lupo che gridava al lupo. Quando arrivavano i *veri* pericoli, tu, giustamente, non mi credevi.

`bb({eyes:"surprise_r"});`

b: Eppure siamo sopravvissuti!

(#act4b)

# act4b

```
bb({eyes:"normal", mouth:"normal"});
hong({eyes:"normal", mouth:"normal"});
```

b: Nonostante tutto, siamo ancora qua.

`hong({eyes:"suspect"});`

{{if _.INJURED}}
h: Sembri piuttosto calmo, considerando che stavamo per morire.
{{/if}}

{{if !_.INJURED}}
h: Sembri piuttosto calmo, considerando che stavamo *quasi* per morire.
{{/if}}

```
hong({eyes:"normal"});
bb({eyes:"annoyed_d", mouth:"narrow"});
```

b: Beh, tutto il resto a confronto fa meno paura. Mi ha fatto anche riflettere.

`bb({eyes:"normal", mouth:"normal"});`

b: Se fa schifo litigare con te, perché non ti tiene al sicuro...

h: Ma *anche* litigare con te fa schifo, perché ti fa abbaiare più forte...

`bb({eyes:"normal_r"})`

b: Forse, allora...

`bb({eyes:"normal"})`

h: Forse non dovremmo litigare.

```
Game.FORCE_CANT_SKIP = true;
Game.clearText();
```

(...301)

`publish("smash",[0]);`

(...2001)

```
publish("smash",[1]);
sfx("smash_glass");
```

(...2601)

```
publish("smash",[2]);
bb({eyes:"normal", mouth:"normal"});
hong({eyes:"normal", mouth:"normal"});
```

(...2001)

`Game.FORCE_CANT_SKIP = false;`

(#act4b_2)

# act4b_2

```
music('dontfight',{fade:5, volume:0.6});
bb({eyes:"annoyed_d"});
```

b: Non sono il lupo cattivo, ma nemmeno un cane da guardia.

`bb({eyes:"sad_d"})`

b: Sono un malconcio cane da rifugio.

`bb({eyes:"sad"})`

b: Abbiamo passato momenti difficili. Forse traumi o negligenze. Ecco perché a volte esagero e faccio:

```
sfx("yaps", {volume:0.6});
bb({body:"yap_1"});
Game.FORCE_CANT_SKIP = true;
Game.WORDS_HEIGHT_BOTTOM = 215;
Game.FORCE_TEXT_DURATION = 90;
Game.FORCE_NO_VOICE = true;
```

b: BLA BLA BLA BLA BLA

(...1884)

```
Game.WORDS_HEIGHT_BOTTOM = -1;
Game.FORCE_CANT_SKIP = false;
bb({body:"normal", mouth:"scream", eyes:"scream_sad"});
```

b: Ma non *voglio* essere un cane fifone! Voglio proteggerti! Voglio essere un bravo cagnolino!

`bb({eyes:"sad", mouth:"normal"});`

b: Tu... mi aiuterai a domare questo lupo?

`hong({eyes:"sad"})`

h: Ci... ci provo.

`hong({eyes:"normal_l", body:"chin", mouth:"narrow"})`

h: Ok. Relazioni sane con le emozioni. Le relazioni necessitano di comunicazione. Quindi, comunichiamo.

`hong({eyes:"normal", body:"hands_1", mouth:"normal"})`

h: I prossimi cinque minuti saranno sdolcinati, ma facciamo finta fino a che non la finiamo.

```
hong({body:"hands_2", mouth:"normal"});
```

h: Caro lupo interiore... come *ti* senti?

n2: TOTALE PAURE USATE:

n2: *FARSI MALE* {{_.attack_harm_total}}, *MANCANZA DI AFFETTO* {{_.attack_alone_total}}, *CATTIVA PERSONA* {{_.attack_bad_total}}

n2: DA QUALE PAURA VORRESTI INIZIARE? (PUOI PARLARE DELLE ALTRE IN SEGUITO)

```
_.a4_fears_discussed = 0;
_.num_thanks = 0;
hong({body:"normal"});
bb({eyes:"normal"});
```

[Paura di farsi male.](#act4_harm)

[Paura di rimanere soli.](#act4_alone)

[Paura di essere cattive persone.](#act4_bad)

# act4_harm

```
_.a4_talked_about_harm = true;
_.a4_fears_discussed += 1;
```

`bb({eyes:"normal_d"})`

b: Voglio proteggerti per la tua incolumità fisica,

`bb({eyes:"sad_d"})`

b: Ma il *mondo intero* sembra pericoloso. Pieno di tragedie e cattiverie.

`bb({eyes:"sad"})`

{{if _.a4_fears_discussed==1}}
b: Non so, sono sempre *io* a decidere cosa dire. *Tu* cosa vorresti dire?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: Tocca di nuovo a te. Cosa ne pensi?
{{/if}}

{{if _.a4_fears_discussed==3}}
b: Altre considerazioni?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Hai ragione. Dobbiamo proteggerci a vicenda.](#act4_harm_skills)

[Dobbiamo esporci a *più* pericoli.](#act4_harm_exposure)

[Grazie.](#act4_thanks) `_.thanks_for = "physical safety";`

# act4_harm_skills

`bb({eyes:"look_down", body:"paw"})`

b: Ma... come? Io ho zanne e artigli, ma solo metaforicamente.

```
bb({ body:"normal", eyes:"normal" });
hong({ body:"one_up", eyes:"surprise" });
```

h: Potremmo imparare l'autodifesa? Unirci a una comunità dove ci si protegge? Migliorare i confini generali e personali di salute?

```
bb({ eyes:"annoyed_r" });
hong({ body:"normal", eyes:"normal" });
```

b: Forse, ma...

[Da dove iniziamo?](#act4_harm_skills_start)

[E se comunque non funzionasse?](#act4_harm_skills_work)

[E se andassimo oltre la "sicurezza"?](#act4_harm_skills_overboard)

# act4_harm_skills_start

`bb({ eyes:"sad_d" })`

b: C'è tanto da fare, dobbiamo sistemare tante cose in noi. Ma da dove *iniziamo*?

`hong({ body:"shrug", eyes:"surprise" })`

h: Abbiamo già iniziato.

`bb({ eyes:"normal", mouth:"narrow" })`

b: Eh?

```
bb({ body:"normal", mouth:"normal" });
hong({ body:"normal", mouth:"normal", eyes:"normal"});
```

h: Ci stiamo esercitando a comunicare proprio ora, il che ci aiuterà a rilevare meglio i pericoli, con meno falsi positivi,

`hong({ eyes:"surprise" });`

h: E *questo* aiuterà a proteggerci dai mali!

`hong({ eyes:"normal", mouth:"normal" });`

h: Perciò ci *stiamo già* esercitando all'autodifesa.

`bb({ eyes:"normal_r" })`

b: Ah, tutto qui?

```
Game.FORCE_CANT_SKIP = true;
Game.clearText();
hong({ eyes:"sad", mouth:"smile" });
bb({ body:"karate_1" });
sfx("hiya");
```

(...1001)

`Game.FORCE_CANT_SKIP = false;`

(#act4_something_else)

# act4_harm_skills_work

`bb({ eyes:"normal" });`

h: Vero, è impossibile proteggerci al 100%...

`hong({ body:"one_up" });`

h: Ma anche un 1% di miglioramento è pur sempre qualcosa, giusto?

```
bb({ eyes:"annoyed" });
hong({ normal:"one_up" });
```

b: Non vedi il bicchiere 99% vuoto, ma lo vedi 1% pieno?

`bb({ eyes:"normal" });`

h: Che è comunque meglio di niente se ti ritrovi in un deserto.

`bb({ eyes:"closed" });`

b: Beh, allora, alla goccia.

(#act4_something_else)

# act4_harm_skills_overboard

`bb({ body:"chest", eyes:"annoyed" })`

b: Cioè, il vero motivo per cui ignoravi i miei avvertimenti era il *mio* andare oltre la sicurezza!

`bb({ body:"normal", eyes:"normal" })`

h: Nah, avevi ragione. Dovremmo fare sicurezza in moderazione. Tutto in moderazione.

`bb({ eyes:"suspect" })`

b: Scusa, *TUTTO* in moderazione?

`hong({ eyes:"annoyed" })`

h: *Un numero moderato di cose* in moderazione.

```
bb({ eyes:"closed" });
hong({ eyes:"normal" });
```

b: Grazie per aver reso le tue affermazioni ricorsivamente coerenti.

(#act4_something_else)


# act4_harm_exposure

`bb({ mouth:"scream_talk", eyes:"scream", MOUTH_LOCK:true });`

b: *COSA*

```
bb({ mouth:"narrow", eyes:"suspect" });
hong({ body:"one_up" });
```

h: Per dire, prendiamo un cane che ha paura dei tuoni.

`hong({ body:"hands_1" });`

h: Un trucchetto degli addestratori è di far sentire un audio dei tuoni a volume basso, per poi premiarlo se rimane calmo.

`hong({ body:"hands_2" });`

h: Giorno dopo giorno, l'addestratore alza piano piano il volume, finché il cane non ha superato la paura dei tuoni.

```
hong({ body:"normal", eyes:"surprise" });
bb({ mouth:"normal", eyes:"normal" });
```

h: Si chiama terapia di esposizione!

`hong({ body:"point", eyes:"normal" });`

h: Sei un cane, dovrebbe funzionare anche con te, no? Tutti i mammiferi hanno la stessa reazione di attacco o fuga.

`hong({ body:"normal" });`

[E se perdessimo *troppa* sensibilità?](#act4_harm_exposure_overboard)

[E se fossimo esposti ad un *vero* pericolo?](#act4_harm_exposure_hurt)

[Sono un lupo, non un cane.](#act4_harm_exposure_dog) `bb({ eyes:"suspect" })`

# act4_harm_exposure_dog

h: Ed io ti mostrerò gentilezza e pazienza finché non diventi un bel cucciolino addomesticato.

`bb({ MOUTH_LOCK:true })`

b: ...

`bb({ eyes:"sad", mouth:"smile" })`

b: Ohh.

(#act4_something_else)

# act4_harm_exposure_overboard

`bb({ eyes:"annoyed" })`

b: Hai visto che succede se ignori le paure? Ci hai fatto cacciare in una situazione *molto* pericolosa.

`bb({ eyes:"angry_r", body:"one_up" })`

b: Inoltre, *troppa* desensibilizzazione non ci renderà degli psicopatici?

`bb({ mouth:"scream", eyes:"scream", body:"two_up" })`

b: Finiremo per sgranocchiarci qualcosa guardando dei porno snuff!

`hong({ eyes:"annoyed" })`

h: Io... credo che ci sia un confine tra quello e i tuoni.

`bb({ body:"normal", mouth:"normal", eyes:"suspect" })`

b: Ma *dove*, esattamente? *Dove*?!

`hong({ eyes:"surprise", body:"one_up" })`

h: Non lo so. Ma *tu* puoi aiutarmi!

`hong({ eyes:"normal", body:"normal" })`

h: Lavorando e negoziando insieme, tracceremo quel confine.

`bb({ body:"paw", mouth:"narrow", eyes:"closed" })`

b: Ok. Ma io non ho i pollici opponibili, dovrai tracciarlo tu.

(#act4_something_else)

# act4_harm_exposure_hurt

`bb({ body:"two_up", eyes:"angry_r" })`

{{if _.INJURED}}
b: Per esempio: siamo saltati da un cavolo di *tetto*!
{{/if}}

{{if !_.INJURED}}
b: Per esempio: stavamo quasi per saltare da un cavolo di *tetto*!
{{/if}}

```
hong({ eyes:"annoyed" });
bb({ body:"normal", eyes:"annoyed" });
```

h: Nah, hai ragione. Si *può* esagerare.

`hong({ eyes:"normal" });`

h: Ma ecco perché, con la terapia di esposizione, inizieremo piano piano, a piccoli passi.

h: Prima di arrivare ai *veri* pericoli, ci fermiamo.

`bb({ eyes:"annoyed_r", mouth:"narrow" });`

b: Ok, traccio il confine tra sentire i tuoni e stare in una tempesta con un lungo cappello a punta.

(#act4_something_else)

# act4_thanks

`_.num_thanks += 1`

{{if _.num_thanks==1}}
(#act4_thanks_1)
{{/if}}

{{if _.num_thanks==2}}
(#act4_thanks_2)
{{/if}}

{{if _.num_thanks==3}}
(#act4_thanks_3)
{{/if}}

# act4_thanks_1

`bb({ MOUTH_LOCK:true })`

b: ...

`bb({ eyes:"annoyed" })`

b: Cosa, nessun commento su come mi sento? Solo... "grazie"?

`hong({ eyes:"surprise", body:"shrug" })`

h: Esatto! Grazie di esserti preoccupato per {{_.thanks_for}}.

```
bb({ eyes:"closed_annoyed", MOUTH_LOCK:true });
hong({ eyes:"normal", body:"normal" });
```

b: ...

h: Tutto bene?

`bb({ eyes:"super_sad", mouth:"narrow" });`

b: Non mi avevi mai *ringraziato* prima d'ora.

`hong({ mouth:"smile" });`

h: Oh, il mio lupone pelosone panicone.

(#act4_something_else)

# act4_thanks_2

h: Anche se esageri, mi fa piacere che ti preoccupi per {{_.thanks_for}}.

`bb({ eyes:"annoyed" })`

b: Aspetta... Non stai continuando a ringraziarmi solo per evitare di parlare delle paure, vero?

```
bb({ eyes:"normal" });
hong({ eyes:"annoyed", body:"chin" });
```

h: Beh, è complicato, e non sempre ho la risposta a tutto.

`hong({ eyes:"annoyed_l", body:"one_up" })`

h: Nella vita non hai una schermata di dialogo con 3 risposte predefinite.

`hong({ eyes:"normal", mouth:"smile", body:"normal" })`

h: Ma per ora, posso almeno dire grazie.

b: Beh, grazie a te, per ascoltarmi pazientemente.

`bb({ eyes:"closed" });`

b: Piccolo mammifero di carne spelacchiato.

(#act4_something_else)

# act4_thanks_3

h: Anche se il tuo blaterare mi mette paura, stai solo provando a proteggere {{_.thanks_for}}.

`bb({ eyes:"smile_r" });`

b: Ok, se continui a lusingarmi così, internet poi si farà strane idee su di noi.

```
bb({ eyes:"smile" });
hong({ eyes:"annoyed" });
```

h: Dai, io una giovane anima vulnerabile e tu un grande lupo spaventoso. Che mai ci può accader-

`hong({ eyes:"normal", body:"point" });`

h: Anzi, meglio non rispondere.

(#act4_something_else)




# act4_alone

```
_.a4_talked_about_alone = true;
_.a4_fears_discussed += 1;
```

`bb({ eyes:"sad_d" });`

b: Voglio assicurarmi che tu soddisfi il bisogno umano di appartenenza,

`bb({ eyes:"sad_u" });`

b: Ma ho paura che se mai qualcuno ci dovesse conoscere *veramente*, li spaventeremmo.

`bb({ eyes:"sad" });`

{{if _.a4_fears_discussed==1}}
b: Non so, sono sempre *io* a decidere cosa dire. *Tu* cosa vorresti dire?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: Tocca di nuovo a te. Cosa ne pensi?
{{/if}}

{{if _.a4_fears_discussed==3}}
b: Altre considerazioni?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Sono d'accordo: lavoriamo sulla nostra vita sociale.](#act4_alone_skills)

[Magari piacciamo agli altri. Vogliamo scoprirlo?](#act4_alone_experiment)

[Grazie.](#act4_thanks) `_.thanks_for = "social belonging";`

# act4_alone_skills

```
bb({ eyes:"normal" });
hong({ body:"chin" });
```

h: Potremmo esercitarci su attività come chiedere, ascoltare, empatizzare, essere aperti e vulnerabili, ecc.

`hong({ eyes:"normal_l" });`

h: O migliorare abitudini come dedicare del tempo per gli amici o andare regolarmente agli incontri?

`hong({ body:"one_up" });`

h: Potremmo anche imparare ad accettare i rifiuti.

`hong({ eyes:"normal" });`

h: O capire che le persone *non* ci rifiutano, se sono stanchi o hanno solo l'espressione imbronciata.

```
hong({ body:"normal" });
bb({ eyes:"annoyed_r" });
```

b: Le opzioni sono tante. Tuttavia, imparare le abilità sociali...

[Non è *manipolazione?*](#act4_alone_skills_manipulative)

[Non ci renderà *più facili da manipolare?*](#act4_alone_skills_manipulated)

[E se non ce la facessimo comunque?](#act4_alone_skills_fail)

# act4_alone_skills_manipulative

`bb({ eyes:"suspect" });`

b: I serial killer sanno capire le emozioni delle vittime, non sono forti in "empatia"?

`bb({ eyes:"annoyed" });`

b: Charles Manson non sapeva come trattare gli altri e farseli amici?

`hong({ eyes:"annoyed", body:"chin" });`

h: No, hai ragione.

h: Le "abilità sociali" non contano se non ci importa davvero *degli* altri.

`hong({ body:"normal" });`

h: In pratica, non fare gli ^stronzi^.

`bb({ eyes:"annoyed", mouth:"smile" });`

b: Là c'è un poster motivazionale.

`hong({ body:"shrug", mouth:"narrow" });`

h: “Non fate gli ^stronzi^™”

(#act4_something_else)

# act4_alone_skills_manipulated

`bb({ eyes:"angry" })`

b: Diventeremo uno zerbino che dice "per favore" e "grazie" quando gli altri ci si puliscono le scarpe!

`bb({ mouth:"scream", eyes:"scream" })`

b: Baceremo così tanti sederi che sembrerà che abbiamo il rossetto marrone!

```
bb({ mouth:"normal", eyes:"normal" });
hong( body:"chin" });
```

h: Nah, hai ragione. Le "abilità sociali" non si trattano solo di compiacere gli altri, ma anche di stabilire dei *confini*.

`hong( body:"one_up" });`

h: Non possiamo invitare persone a casa, se non abbiamo delle mura che la sorreggano.

```
hong( eyes:"angry", mouth:"narrow" });
bb( eyes:"annoyed", mouth:"smile" });
```

h: Poi... quella cosa del rossetto... *che schifo*!!

(#act4_something_else)

# act4_alone_skills_fail

`bb({ eyes:"annoyed" });`

h: Potremmo fallire. Anzi, *falliremo*.

```
bb({ eyes:"normal" });
hong({ eyes:"surprise", body:"shrug" });
```

h: E va bene così! È fallendo che si impara qualcosa di nuovo!

`hong({ body:"normal", eyes:"normal" });`

h: Quindi falliamo insieme, ok?

`bb({ eyes:"normal_r" });`

b: Immagino di sì... Alle brutte, possiamo cambiare città e farci una nuova identità.
`bb({ eyes:"normal" });`

h: Sì, forse ad oggi costerà giusto un paio di bitcoin.

(#act4_something_else)

# act4_alone_experiment

```
hong({ body:"one_up" });
bb({ eyes:"normal" });
```

h: Possiamo provare a sperimentare!

`hong({ body:"chin" });`

h: Chiedere a un amico di uscire, risentire vecchie conoscenze, o scambiare due parole con i baristi.

`hong({ body:"normal" });`

h: Magari scopriamo di essere più simpatici del previsto.

`bb({ eyes:"annoyed" });`

[E se fossero dei piccoli "successi" da poco?](#act4_alone_experiment_cheap)

[E se fosse un peso per gli altri?](#act4_alone_experiment_burden)

[Ma parlare del più e del meno non è *da noi*!](#act4_alone_experiment_real_us)

# act4_alone_experiment_real_us

`bb({ eyes:"sad" });`

b: Se sorridiamo forzatamente, non riusciremo mai a comunicare con nessuno,

`bb({ eyes:"super_sad" });`

b: *Ma* se ci apriamo, gli altri vedranno tutto il nostro disordine interno!

`hong({body:"chin", mouth:"narrow", MOUTH_LOCK:true})`

h: ...

```
hong({body:"normal", mouth:"normal"});
bb({eyes:"normal"});
```

h: Rotola.

b: Cosa.

`hong({body:"hands_1"})`

h: Quando i cani vogliono esprimere amore e fiducia, si rendono vulnerabili mostrando la pancia.

`hong({body:"one_up"})`

h: Forse non siamo *ancora* al sicuro per essere vulnerabili, ma con la pratica,

`hong({body:"normal", eyes:"surprise"})`

h: Un giorno riusciremo a mostrarci per come siamo: disastrati, ma umani.

```
hong({eyes:"normal"});
bb({ eyes:"super_sad", mouth:"smile", body:"chest" });
```

b: Rotolerò se mi dai un biscottino.

`bb({ eyes:"normal", mouth:"normal" });`

h: No.

(#act4_something_else)


# act4_alone_experiment_cheap

b: Dire "ciao" a chi lavora al bar non è proprio una prestazione da medaglia d'oro alle Socialimpiadi.

```
hong({ body:"point", eyes:"surprise" });
bb({ eyes:"normal" });
```

h: Per *noi* lo è!

`hong({ body:"one_up", eyes:"annoyed" });`

h: Nel ring sociale, non siamo nemmeno peso piuma, siamo tipo... peso ricotta.

`hong({ body:"normal", eyes:"normal" });`

h: Dobbiamo iniziare con piccoli successi da poco. Solo facendo il primo passo si arriva al millesimo.

b: Esatto! Dopo aver detto "ciao", possiamo proseguire con...

`bb({ body:"two_up", mouth:"smile", eyes:"smile_u" });`

b: *"Come stai?"*

`hong({ body:"shrug", mouth:"smile", eyes:"surprise_l" });`

h: *"Non c'è male!*

(#act4_something_else)

# act4_alone_experiment_burden

`bb({ eyes:"suspect_r" })`

b: Forse vuole solo fare un dannato caffè, non diventare *cavia* dei nostri fallimenti nelle interazioni sociali.

`bb({ eyes:"annoyed" })`

h: Beh, se venisse fuori che *siamo* un peso...

```
hong({ eyes:"surprise" });
bb({ eyes:"normal" });
```

h: Comunque buono a sapersi!

`hong({ eyes:"normal" });`

h: Possiamo imparare a chiedere proattivamente agli altri cosa li mette a proprio agio, per conoscere e rispettare i confini.

```
hong({ eyes:"annoyed_l", mouth:"narrow" });
bb({ eyes:"annoyed", mouth:"smile" });
```

h: Sai, quella robaccia delle "abilità relazionali" sui volantini dei consulenti.

(#act4_something_else)



# act4_bad

```
_.a4_talked_about_bad = true;
_.a4_fears_discussed += 1;
```

`bb({ eyes:"annoyed_r" })`

b: Voglio difendere i tuoi bisogni morali, che ti rendono una persona migliore,

`bb({ eyes:"sad_d" })`

b: Ma sento che, in fondo, siamo completamente... rotti.

`bb({ body:"two_up", eyes:"angry" })`

{{if _.INJURED}}
b: E non dirmi che *non* siamo incasinati. Siamo saltati da un *tetto*.
{{/if}}

{{if !_.INJURED}}
b: E non dirmi che *non* siamo incasinati. Siamo quasi saltati da un *tetto*.
{{/if}}

`bb({ body:"normal", eyes:"sad" })`

{{if _.a4_fears_discussed==1}}
b: Non so, sono sempre *io* a decidere cosa dire. *Tu* cosa vorresti dire?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: Tocca di nuovo a te. Cosa ne pensi?
{{/if}}

{{if _.a4_fears_discussed==3}}
b: Altre considerazioni?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Dunque, siamo rotti. Rimediamo.](#act4_bad_fix)

[Dunque, siamo rotti. Accettiamolo.](#act4_bad_accept)

[Grazie.](#act4_thanks) `_.thanks_for = "moral well-being";`

# act4_bad_fix

```
bb({eyes:"normal"});
hong({body:"chin"});
```

h: Potremmo piano piano crearci abitudini migliori, vivere seguendo i nostri valori.

`hong({body:"one_up"});`

h: E in caso chiedere un aiuto professionale: uno psicologo o un consulente.

`hong({body:"normal"});`

h: I modi per uscirne ci sono.

[E se non riuscissimo a uscirne del tutto?](#act4_bad_fix_cant)

[E se ne uscissimo *fin* troppo?](#act4_bad_fix_too_much)

[Non possiamo permetterci un aiuto professionale.](#act4_bad_fix_afford)

# act4_bad_fix_cant

`hong({eyes:"annoyed"});`

h: Nah, forse hai ragione.

h: Non possiamo uscirne del tutto.

`bb({mouth:"scream", eyes:"scream_sad"});`

b: Ahhh lo sapevo, saremo per sempre rotti!

`hong({eyes:"surprise"});`

h: Ma almeno possiamo essere *meno* rotti.

```
bb({mouth:"normal", eyes:"annoyed"});
hong({eyes:"sad", mouth:"smile"});
```

h: Le cicatrici col tempo guariscono, ma non se ne andranno. E va bene così.

`bb({eyes:"annoyed_r"});`

b: Credo di sì. E poi,

```
Game.FORCE_TEXT_Y = 460;
Game.clearText();
publish("act4-sexy", [true]);
```

b: Le cicatrici sono *sexy*.

```
Game.FORCE_TEXT_Y = -1;
Game.clearText();
publish("act4-sexy", [false]);
bb({body:"chest", mouth:"smile_talk", MOUTH_LOCK:true, eyes:"sexy"}, 0);
hong({eyes:"normal", mouth:"normal"}, 0);
```

h: Ti prego, no.

(#act4_something_else)

# act4_bad_fix_too_much

`bb({ eyes:"angry_d" })`

b: Fa male ammetterlo, ma... una parte di me *vuole* avere questo disturbo.

`bb({ eyes:"angry" })`

b: Cioè, non diventeremo *noiosi* senza?

`bb({ eyes:"sad_r", body:"one_up" })`

b: Senza, non è che la nostra arte diventa banale ed insipida?

`bb({ eyes:"sad_u", body:"two_up" })`

b: Senza, non è che non saremo più in grado di stare con gli amici che hanno questo disturbo?

`bb({ eyes:"sad", body:"chest" })`

b: Se mai saremo soddisfatti della vita, non è che smetteremo di fare grandi cose?

`hong({ MOUTH_LOCK:true })`

h: ...

h: Se abbiamo persino paura... di "scappare dalle paure"...

h: Non credo riusciremo a scappare.

`bb({ eyes:"smile_u", body:"normal", mouth:"smile" })`

b: Oh, sì! Uh, che sollievo!

(#act4_something_else)

# act4_bad_fix_afford

`bb({ body:"one_up", eyes:"sexy", mouth:"normal" })`

b: "Guardi, ho l'ansia di pagare 100$ l'ora solo per farmi chiedere *questo come ti fa sentire?*"

`bb({ body:"paw", eyes:"closed", mouth:"narrow" })`

b: "Mm-hmm. E questo come ti fa sentire?"

```
bb({ body:"normal", eyes:"normal", mouth:"normal" });
hong({ eyes:"sad" });
```

h: Nah, è comprensibile che ti preoccupi.

`hong({ eyes:"annoyed", mouth:"sad" });`

h: E fa veramente schifo il fatto che la sanità mentale per tanta gente sia un lusso.

`hong({ eyes:"normal", mouth:"normal" });`

h: Ma ci sono anche opzioni economiche o gratuite:

`hong({ body:"chin" })`

h: Gruppi di supporto, terapia online, centri sanitari per studenti o a scopo di lucro...

`hong({ body:"hands_1" })`

h: Sviluppare abitudini come meditare, dormire bene, chattare regolarmente con gli amici, imparare cose nuove,

`hong({ body:"hands_2" })`

h: Prendere in prestito dalla biblioteca manuali per psicoterapia basata sull'evidenza,

`hong({ body:"one_up" })`

h: Alla fine c'è una lunga lista di risorse!

```
hong({ body:"normal" });
bb({ eyes:"annoyed", mouth:"narrow" });
```

b: Beh, *quella* quarta parete non è durata molto.

`hong({ body:"point" });`

h: Ci sono cose più importanti delle regole di narrazione. Come la salute mentale.

(#act4_something_else)


# act4_bad_accept

```
bb({ eyes:"normal" });
hong({ eyes:"normal_l", body:"one_up", mouth:"narrow" });
```

h: Insomma, è quello che dicono gli psicologi, no? Accettare i sentimenti, anche quelli negativi?

```
bb({ eyes:"annoyed" });
hong({ eyes:"normal", body:"normal", mouth:"normal" });
```

b: Aspetta.

["Accettare" nel senso di *arrendersi*?](#act4_bad_accept_give_up)

["Accettare" nel senso di *approvare*?](#act4_bad_accept_approve)

["Accettare" *inteso letteralmente*?](#act4_bad_accept_literally)

# act4_bad_accept_give_up

`bb({ eyes:"angry", body:"one_up" });`

b: Pensi che Martin Luther King abbia detto: "Caspita, non possiamo sederci ai posti davanti del bus, *pazienza*!"?

`bb({ eyes:"angry_r", body:"two_up" });`

b: Perché il Complesso Industriale dell'Auto-Aiuto pensa che arrendersi sia *profondamente saggio*?

`bb({ eyes:"annoyed", body:"normal" });`

h: Penso che gli psicologi con "accettare" le cose brutte intendano: ammetterne l'esistenza e l'inflessibilità,

h: Ma non per forza arrendersi al tentativo di cambiarle.

`bb({ eyes:"suspect" });`

b: Allora gli psicologi dovrebbero dire *riconoscere*, non *accettare*.

`hong({ body:"chin", eyes:"annoyed" });`

h: Sì, ora che ci penso, *accettare* è abbastanza fuorviante.

`bb({ eyes:"closed", mouth:"narrow" });`

b: Beh, lo *riconosco*.

(#act4_something_else)

# act4_bad_accept_approve

`bb({ eyes:"angry" });`

b: Cioè, va *bene* essere rotti o qualcosa del genere? No!

`bb({ eyes:"angry_r", body:"one_up" });`

b: Gli sceneggiatori che romanticizzano i disturbi mentali hanno la segatura nel cervello!

`bb({ eyes:"angry", body:"two_up" });`

b: Avere un disturbo mentale *fa schifo*! Deruba le persone della *vita*! Perché dovremmo *accettarlo*?

`bb({ body:"normal" });`

h: Penso che gli psicologi con "accettare" le emozioni intendano: averci pazienza.

```
hong({ body:"one_up" });
bb({ eyes:"normal" });
```

h: Come quando agitarsi nelle sabbie mobili ti fa affondare più veloce, e la soluzione è stendersi pazientemente.

`hong({ eyes:"surprise" });`

{{if _.INJURED}}
h: Lottare contro di te, la mia paura, mi ha fatto saltare da un tetto.
{{/if}}

{{if !_.INJURED}}
h: Lottare contro di te, la mia paura, mi ha quasi fatto saltare da un tetto.
{{/if}}

`hong({ body:"normal", eyes:"normal" });`

h: Invece, la soluzione è quello che stiamo facendo adesso: non lottare, ma essere pazienti l'un con l'altro.

`bb({ eyes:"annoyed" });`

b: Allora *questo* dovrebbero dire, non parole problematiche come "accettare".

`hong({ body:"chin", eyes:"annoyed" });`

h: Sì, ora che ci penso, *accettare* fa abbastanza schifo.

`bb({ eyes:"closed_annoyed", mouth:"narrow" });`

b: Non accetto "accettare".

(#act4_something_else)

# act4_bad_accept_literally

`bb({ eyes:"sad", body:"one_up" });`

b: Ma noi *sappiamo* già che non dovresti prendermi alla lettera!

`bb({ eyes:"sad_u", body:"two_up" });`

b: Il vero *problema* è che voglio aiutarti, ma faccio schifo nel farlo a parole.

`bb({ eyes:"sad", body:"normal" });`

h: Penso che gli psicologi per "accettare" le emozioni intendano: non lottarci o ignorarli.

`hong({ eyes:"surprise", body:"one_up" });`

h: Per ascoltarti, lavorare *con* te, non prendere 100% vero tutto quello che dici.

```
hong({ eyes:"normal", body:"normal" });
bb({ eyes:"annoyed", mouth:"normal" });`
```

b: Allora dovrebbero dire *questo* anziché parole vaghe e fuorvianti come "accettare".

`hong({ body:"chin", eyes:"annoyed" });`

h: Immagino anche loro facciano schifo a parole.

(#act4_something_else)




# act4_something_else

```
bb({ body:"normal", mouth:"normal", eyes:"normal" });
hong({ body:"normal", mouth:"normal", eyes:"normal" });
```

{{if _.a4_fears_discussed==1}}
h: Comunque, altro di cui vuoi parlare?
{{/if}}

{{if _.a4_fears_discussed==2}}
h: Allora, altro di cui vuoi sfogarti?
{{/if}}

{{if _.a4_fears_discussed==3}}
(#act4_something_else_2)
{{/if}}

{{if _.a4_talked_about_harm!=true}}
[Ho paura che ci faremo male.](#act4_harm)
{{/if}}

{{if _.a4_talked_about_alone!=true}}
[Ho paura che rimarremo soli.](#act4_alone)
{{/if}}

{{if _.a4_talked_about_bad!=true}}
[Ho paura che siamo delle cattive persone.](#act4_bad)
{{/if}}

[Nah, per ora sto bene.](#act4c_prelude)

# act4_something_else_2

h: Ok, credo che abbiamo parlato di tutte le nostre paure.

b: Sì, sono solo tre paure.

h: Già, proprio tre.

b: Ottimo direi.

(#act4c)

# act4c_prelude

h: Bella chiacchierata.

(#act4c)

# act4c

```
Game.clearText();
music(null,{fade:3});
bb({body:"normal", eyes:"normal", mouth:"normal", MOUTH_LOCK:true},0);
hong({body:"normal", eyes:"normal", mouth:"normal"},0);
```

b: ...

`hong({MOUTH_LOCK:true},0)`

h: ...

`bb({eyes:"annoyed_d"})`

b: Non è un *gioco*, lo sai.

`bb({eyes:"angry_d", body:"one_up"})`

b: Instaurare una relazione sana con le proprie emozioni non è facile come fare clic su uno schermo.

`bb({eyes:"sad", body:"normal"})`

b: *Possiamo* davvero andare d'accordo?

b: *Possiamo* lavorare insieme, come una squadra?

`hong({eyes:"sad", body:"one_up"})`

h: Beh,

```
hong({eyes:"surprise_l"});
bb({eyes:"normal"});
```

a: S-scusa...

```
Game.clearText();
publish("act4-in-2");
music('campus', {volume:0.5, fade:1});
```

(...2101)

(#act4d)

# act4d

`Game.WORDS_HEIGHT_BOTTOM = 221;`

`publish("act4", ["alshire", 0]);`

a: P-posso sedermi a mangiare vicino a te? 

`publish("act4", ["alshire", 1]);`

{{if _.TOP_FEAR=="harm"}}
s: Ma non è la tua cotta? Perché si siede per conto suo come i serial killer?
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: Chiedere alla tua cotta se ti ci puoi sedere vicino? Non ti suona così *disperato*?
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: Ma non è la tua cotta? Abbiamo interrotto la sua pace e quiete! Siamo un peso!
{{/if}}

`publish("act4", ["alshire", 2]);`

a: C-cioè, sennò fa... fa niente, io...

`publish("act4", ["alshire", 3]);`

`Game.OVERRIDE_CHOICE_SPEAKER = "h2"`

[Aspetta, io ti ho visto alla festa!](#act4d_recognition) `publish("act4", ["hong_to_alshire",1])`

[Sì, certo! Vieni.](#act4d_yes) `publish("act4", ["hong_to_alshire",2])`

[Scusa, vorrei stare per conto mio.](#act4d_no) `publish("act4", ["hong_to_alshire",8])`

# act4d_recognition

`publish("act4", ["hong_to_alshire",2]);`

h2: Sì, stavi sul divano! Alla prima festa a cui ho partecipato!

`publish("act4", ["hong_to_alshire",10]);`

{{if _.a2_ending=="fight"}}
h2: Ho avuto l'attacco di panico e preso a pugni l'ospitante.
{{/if}}

{{if _.a2_ending=="flight"}}
h2: Ho avuto l'attacco di panico scappando poi in lacrime.
{{/if}}

```
publish("act4", ["hong_to_alshire", 0]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: Aspetta, così potrebbe stare a disagio.

```
publish("act4", ["hong_to_alshire", 3]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: Ah, non voglio metterti alle strette!

`publish("act4", ["hong_to_alshire",4]);`

h2: Solo avevo riconosciuto una faccia amica, tutto qua.

```
publish("act4", ["hong_to_alshire",5]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: AHHHHH LO SAPEVO! UNA PERSONA PERICOLOSA PSICOPATICA!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: AAHHH LA SUA PRIMA IDEA SU DI NOI È STATA "HA ASSISTITO AL MIO TRAUMA"! ORA CI ODIA!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: AAHH ABBIAMO FATTO SBLOCCARE UN EVENTO TRAUMATICO. LA NOSTRA SOLA PRESENZA FERISCE TUTTI.
{{/if}}

(#act4e)

# act4d_yes

```
publish("act4", ["hong_to_alshire", 5]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: Aspetta, sembra essere a disagio.
```
publish("act4", ["hong_to_alshire", 6]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: Ah, non voglio metterti sotto pressione.

`publish("act4", ["hong_to_alshire", 4]);`

h2: Volevo dire, puoi sederti qui, se vuoi.

```
publish("act4", ["hong_to_alshire", 5]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: È *TROPPO* AMICHEVOLE! COME TED BUNDY, IL SERIAL KILLER!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: È SOLO GENTILE! NESSUNO VUOLE *VERAMENTE* STARCI VICINO!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: AHHH METTIAMO SEMPRE TUTTI IN IMBARAZZO! SIAMO UNA PIAGA DELLA SOCIETÀ!
{{/if}}

(#act4e)

# act4d_no

```
publish("act4", ["hong_to_alshire", 9]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: Aspetta, potrebbe sentirsi di troppo.

```
publish("act4", ["hong_to_alshire", 3]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: Ah, non volevo essere rude!

`publish("act4", ["hong_to_alshire", 6]);`

h2: Ho solo bisogno di un po' di tempo per elaborare le mie emozioni. Non prenderla sul personale.

```
publish("act4", ["hong_to_alshire", 7]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: CHE PENSIERI DEVIATI STA ELABORANDO?! QUALI DESIDERI OSCURI COLMANO IL CUORE DI TALE FOLLE?!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: CI HA PERSONALMENTE RIFIUTATI! NON CI AMERÀ MAI NESSUNO!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: ABBIAMO INTERROTTO LA SUA ELABORAZIONE EMOTIVA! ORA RIMARRÀ COL TRAUMA A VITA ED È TUTTA COLPA NOSTRA!
{{/if}}

(#act4e)

# act4e

```
Game.WORDS_HEIGHT_BOTTOM = 195;
publish("act4", ["alshire", 6]);
```

s: SCAPPA SCAPPA SCAPPA SCAPPA SCAPPA SCAPPA SCAPPA SCAPPA

```
Game.clearText();
publish("act4", ["hong_to_alshire", 0]);
publish("act4", ["alshire", 10]);
sfx("pop");
```

(...1001)

```
publish("act4", ["alshire", 11]);
sfx("alshire_run");
```

(...2601)

```
publish("act4-out-3");
Game.WORDS_HEIGHT_BOTTOM = -1; /* reset */
```

(...1201)

`publish("act4-jumpcut-hong");`

h: Uh. È stato strano. Chissà che gli ronzava nella testa.

`publish("act4", ["hong_closer", 2]);`

h: Comunque, dicevi?

```
publish("act4", ["hong_closer", 1]);
publish("act4", ["bb_closer", 6]);
```

b: Ehm, non ricordo... Qualcosa su lavoro e squadra?

```
publish("act4", ["bb_closer", 0]);
publish("act4", ["hong_closer", 3]);
```

h: ¯\_(ツ)_/¯

```
publish("act4", ["hong_closer", 1]);
publish("act4", ["bb_closer", 4]);
```

b: Dicono che dovresti "fare pace" con le emozioni, come se fossero dei *criminali di guerra*.

`publish("act4", ["bb_closer", 7]);`

b: Ma io voglio *più* di una semplice pace! Voglio che diventiamo *alleati*!

`publish("act4", ["bb_closer", 3]);`

b: Voglio essere un buon cane da guardia. Come fame e sete sono allarmi per i tuoi bisogni fisici,

`publish("act4", ["bb_closer", 8]);`

b: Voglio essere l'allarme per i tuoi bisogni *psicologici*: sicurezza, appartenenza, bontà.

`publish("act4", ["bb_closer", 1]);`

b: Ma... faccio schifo nel farlo, quindi devi addestrarmi.

`publish("act4", ["bb_closer", 4]);`

b: Non sono "sempre valido", né "sempre irrazionale". Faccio solo... del mio meglio. Quindi...

`publish("act4", ["bb_closer", 30]);`

b: Aiutami ad aiutarti!

`publish("act4", ["bb_closer", 6]);`

b: Anche se per riaddestrare un cane anziano *ci vorrà* un po'. Forse *anni*.

`publish("act4", ["bb_closer", 3]);`

b: E a volte ricadrò nelle vecchie abitudini.

`publish("act4", ["bb_closer", 2]);`

b: Abbaierò alle ombre. Ti spaventerò con le parole. Potrei persino mostrarti immagini intrusive di... cose.

`publish("act4", ["bb_closer", 9]);`

b: Scusa! Sono un malconcio cane da rifugio, di quelli che ti fanno i bisogni sul letto!

`publish("act4", ["bb_closer", 4]);`

b: Ma se sei paziente con me... e rimani qui con me...

`publish("act4", ["bb_closer", 8]);`

b: Forse puoi domare questo lupo.

`publish("act4", ["bb_closer", 0]);`

`Game.clearText();`

(...1000)

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Bravo cagnolino.](#act4f-pat-bb) `Game.OVERRIDE_CHOICE_SPEAKER = "h"; publish("act4", ["hong_closer", 2]);`

`Game.OVERRIDE_CHOICE_SPEAKER = "b"`

[Bravo umano.](#act4f-pat-hong) `Game.OVERRIDE_CHOICE_SPEAKER = "b"; publish("act4", ["bb_closer", 8]);`

# act4f-pat-hong

```
Game.clearText();
publish("hide_tabs");
Game.FORCE_CANT_SKIP = true;
music(null,{fade:0.5});
sfx("youbothwin");
```

```
publish("act4", ["hong_closer", 4]);
publish("act4", ["bb_closer", 13]);
```

(...501)

`publish("act4", ["bb_closer", 14]);`

(...501)

`publish("act4", ["bb_closer", 13]);`

(...501)

`publish("act4", ["bb_closer", 14]);`

(...501)

`publish("act4", ["bb_closer", 13]);`

(...501)

`publish("act4", ["bb_closer", 14]);`

(...6501)

`publish("act4", ["bb_closer", 15]);`

(...1001)

(#act4f)

# act4f-pat-bb

```
Game.clearText();
publish("hide_tabs");
Game.FORCE_CANT_SKIP = true;
music(null,{fade:0.5});
sfx("youbothwin");
```

```
publish("act4", ["hong_closer", 4]);
publish("act4", ["bb_closer", 10]);
```

(...501)

`publish("act4", ["bb_closer", 11]);`

(...501)

`publish("act4", ["bb_closer", 10]);`

(...501)

`publish("act4", ["bb_closer", 11]);`

(...501)

`publish("act4", ["bb_closer", 10]);`

(...501)

`publish("act4", ["bb_closer", 11]);`

(...6501)

`publish("act4", ["bb_closer", 12]);`

(...1001)

(#act4f)

# act4f

```
Game.FORCE_CANT_SKIP = false;
publish("act4", ["bb_closer", 16]);
publish("act4", ["hong_closer", 5]);
```

{{if _.fifteencigs}}
b: AAAAA STAI ANCORA PER CONTO TUO QUINDICI SIGARETTE AAAAA
{{/if}}

{{if _.parasite}}
b: AAAAA NON STAI ANCORA FACENDO NULLA MENTRE MANGI SIAMO PARASSITI SOCIALI AAAAA
{{/if}}

{{if _.whitebread}}
b: AAAAA STAI MANGIANDO ANCORA PANE BIANCO AAAAA
{{/if}}

```
publish("act4", ["bb_closer", 18]);
publish("act4", ["hong_closer", 6]);
sfx("yaps", {volume:0.6});
Game.FORCE_CANT_SKIP = true;
Game.WORDS_HEIGHT_BOTTOM = 205;
Game.FORCE_TEXT_DURATION = 90;
Game.FORCE_NO_VOICE = true;
```

b: BLA BLA BLA BLA BLA

(#credits)
