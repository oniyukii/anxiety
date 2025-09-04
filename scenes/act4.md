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

n3: (gioco salvato automaticamente)

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

h: Cosa abbiamo *imparato*? Mi *stavo* comportando da idiota, i miei "amici" mi *stavano* usando, e stavamo quasi per *morire*, cavolo.

`hong({body:"normal", eyes:"normal"})`

{{if _.INJURED}}
[Già, per non parlare delle spese mediche.](#act4a_bill)
{{/if}}

{{if !_.INJURED}}
[Già, per non parlare del danno epatico.](#act4a_liver)
{{/if}}

[Già, quello *è stato* il peggio che potesse capitare](#act4a_worst)

[Già, avevo ragione.](#act4a_right)

# act4a_bill

`hong({eyes:"annoyed_l", mouth:"narrow"});`

h: Vero. Non penso il piano assicurativo copra la polizza "sono un idiota".

`hong({eyes:"annoyed", mouth:"normal"});`

b: Eppure... siamo sopravvissuti!

`hong({eyes:"normal"});`

h: ?

(#act4b)

# act4a_liver

`bb({eyes:"normal_d"});`

b: Abbiamo decisamente perso qualche anno di vita...

`bb({eyes:"surprise"});`

b: Ma almeno ce l'*abbiamo* ancora, qualche anno di vita! Siamo sopravvissuti!

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

b: Io *ero* il lupo che gridava al lupo al lupo. Perciò, quando arrivavano i *veri* pericoli, tu, giustamente, non mi credevi.

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
h: Sembri piuttosto calmo, considerando che stavamo *tanto così* per morire.
{{/if}}

```
hong({eyes:"normal"});
bb({eyes:"annoyed_d", mouth:"narrow"});
```

b: Beh, tutto il resto a confronto fa meno paura. Mi ha fatto anche riflettere.

`bb({eyes:"normal", mouth:"normal"});`

b: Se io faccio schifo a litigare con te, perché non riesco a proteggerti...

h: Ma *anch'io* faccio schifo a litigare con te, perché ti faccio solo abbaiare più forte...

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

b: Non sono il lupo cattivo, ma non sono nemmeno un lupo da guardia.

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

b: Umano... mi aiuterai a domare questo lupo?

`hong({eyes:"sad"})`

h: Ci... ci provo.

`hong({eyes:"normal_l", body:"chin", mouth:"narrow"})`

h: Ok. Relazioni sane con le emozioni. Le relazioni necessitano di comunicazione. Quindi, comunichiamo.

`hong({eyes:"normal", body:"hands_1", mouth:"normal"})`

h: I prossimi cinque minuti saranno sdolcinati, ma facciamo finta fino a che non finiamo.

```
hong({body:"hands_2", mouth:"normal"});
```

h: Caro lupo interiore... come *ti* senti?

n2: TOTALE PAURE USATE:

n2: *STARE MALE* {{_.attack_harm_total}}, *NON RICEVERE AFFETTO* {{_.attack_alone_total}}, *CATTIVA PERSONA* {{_.attack_bad_total}}

n2: DI QUALE PAURA VORRESTI PARLARE PER PRIMA? (PUOI PARLARE DELLE ALTRE IN SEGUITO)

```
_.a4_fears_discussed = 0;
_.num_thanks = 0;
hong({body:"normal"});
bb({eyes:"normal"});
```

[Paura di stare male.](#act4_harm)

[Paura di rimanere da soli.](#act4_alone)

[Paura di essere cattive persone.](#act4_bad)

# act4_harm

```
_.a4_talked_about_harm = true;
_.a4_fears_discussed += 1;
```

`bb({eyes:"normal_d"})`

b: Voglio proteggerti per la tua incolumità fisica,I want to protect your need for physical safety,

`bb({eyes:"sad_d"})`

b: Ma il *mondo intero* sembra pericoloso. Pieno di tragedie e cattiverie.

`bb({eyes:"sad"})`

{{if _.a4_fears_discussed==1}}
b: Non so, enough of *me* choosing what to say next. *Tu* che ne dici, umano?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: Adesso tocca a te, umano. Che ne pensi?
{{/if}}

{{if _.a4_fears_discussed==3}}
b: Altro da dire, umano?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Hai ragione. Dobbiamo proteggerci a vicenda.](#act4_harm_skills)

[Dobbiamo esporci a *più* pericoli.](#act4_harm_exposure)

[Grazie.](#act4_thanks) `_.thanks_for = "physical safety";`

# act4_harm_skills

`bb({eyes:"look_down", body:"paw"})`

b: Ma... come? Io ho zanne e artigli, ma sono solo un concetto.

```
bb({ body:"normal", eyes:"normal" });
hong({ body:"one_up", eyes:"surprise" });
```

h: Potremmo imparare l'autodifesa? Unirci a una comunità dove ci si protegge a vicenda? Migliorare i nostri confini generali e personali di salute?

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

b: C'è tanto da fare, dobbiamo sistemare tante cose di noi. Da dove *iniziamo*?

`hong({ body:"shrug", eyes:"surprise" })`

h: Abbiamo già iniziato.

`bb({ eyes:"normal", mouth:"narrow" })`

b: Eh?

```
bb({ body:"normal", mouth:"normal" });
hong({ body:"normal", mouth:"normal", eyes:"normal"});
```

h: Proprio ora, ci stiamo esercitando a comunicare, il che ci aiuterà a rilevare meglio i pericoli, con meno falsi positivi,

`hong({ eyes:"surprise" });`

h: E *questo* ci aiuterà a proteggerci dai mali!

`hong({ eyes:"normal", mouth:"normal" });`

h: Perciò: questo *è già* addestramento di autodifesa.

`bb({ eyes:"normal_r" })`

b: Huh. I was expecting more of this:

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

h: Vero, è impossibile proteggerci al 100%...True, there's no way to 100% protect ourselves...

`hong({ body:"one_up" });`

h: Ma anche un 1% di miglioramento è pur sempre qualcosa, giusto?

```
bb({ eyes:"annoyed" });
hong({ normal:"one_up" });
```

b: Non vedi il bicchiere 99% vuoto, ma lo vedi 1% pieno??You're seeing the glass as not 99% empty, but 1% full?

`bb({ eyes:"normal" });`

h: Che è meglio di niente se stai morendo di sete in un deserto.Which is still worth something if you're stranded in the desert.

`bb({ eyes:"closed" });`

b: Beh, allora, su il bicchiere.Well. Bottoms up, then.

(#act4_something_else)

# act4_harm_skills_overboard

`bb({ body:"chest", eyes:"annoyed" })`

b: Cioè, il vero motivo per cui ignoravi i miei segnali era il *mio* andare oltre la sicurezza!I mean, the whole reason you ignored my warnings was because *I* went overboard with safety! 

`bb({ body:"normal", eyes:"normal" })`

h: Nah, avevi ragione. Dovremmo fare sicurezza in moderazione. Tutto in moderazione. Naw, you're right. We would want to do safety in moderation. Everything in moderation.

`bb({ eyes:"suspect" })`

b: Scusa, *TUTTO* in moderazione?

`hong({ eyes:"annoyed" })`

h: *Un numero moderato di cose* in moderazione.

```
bb({ eyes:"closed" });
hong({ eyes:"normal" });
```

b: Thank you for making your statements recursively self-consistent.

(#act4_something_else)


# act4_harm_exposure

`bb({ mouth:"scream_talk", eyes:"scream", MOUTH_LOCK:true });`

b: *COSA*

```
bb({ mouth:"narrow", eyes:"suspect" });
hong({ body:"one_up" });
```

h: Nel senso, prendiamo un cane che ha paura dei tuoni.I mean, let's say a dog is scared of thunder.

`hong({ body:"hands_1" });`

h: Un trucchetto usato dagli addestratori è quello di riprodurre la registrazione dei tuoni a volume basso, poi premiano il cane per essere rimasto calmo.

`hong({ body:"hands_2" });`

h: Giorno dopo giorno, l'addestratore alza piano piano il volume, finché il cane non ha superato la paura dei tuoni.

```
hong({ body:"normal", eyes:"surprise" });
bb({ mouth:"normal", eyes:"normal" });
```

h: Si chiama terapia di esposizione!

`hong({ body:"point", eyes:"normal" });`

h: Tu sei un cane, quindi dovrebbe funzionare anche con te, giusto? Tutti i mammiferi hanno la stessa reazione di attacco o fuga.

`hong({ body:"normal" });`

[What if we desensitize *too* much?](#act4_harm_exposure_overboard)

[E se siamo esposti ad un *vero* pericolo?](#act4_harm_exposure_hurt)

[Sono un lupo, non un cane.](#act4_harm_exposure_dog) `bb({ eyes:"suspect" })`

# act4_harm_exposure_dog

h: Ed io ti mostrerò gentilezza e pazienza fino a farti diventare un bel cucciolino addomesticato.And I'll show you kindness and patience 'til you're domesticated into a cute lil' puppy.

`bb({ MOUTH_LOCK:true })`

b: ...

`bb({ eyes:"sad", mouth:"smile" })`

b: Ohh.

(#act4_something_else)

# act4_harm_exposure_overboard

`bb({ eyes:"annoyed" })`

b: Abbiamo *appena* visto cosa succede se metti a tacere le paure... ci hai fatto cacciare in una situazione *veramente* pericolosa.

`bb({ eyes:"angry_r", body:"one_up" })`

b: Inoltre, won't *too* much desensitization turn us into psychopaths?

`bb({ mouth:"scream", eyes:"scream", body:"two_up" })`

b: Soon we'll give ourselves treats while watching snuff murder porn!

`hong({ eyes:"annoyed" })`

h: Io... credo che quello sia molto diverso dai tuoni.

`bb({ body:"normal", mouth:"normal", eyes:"suspect" })`

b: Ma *dove*, esattamente? *Dove*?!

`hong({ eyes:"surprise", body:"one_up" })`

h: Non lo so. Ma *tu* puoi aiutarmi!

`hong({ eyes:"normal", body:"normal" })`

h: Working and negotiating with you, we'll draw that line.

`bb({ body:"paw", mouth:"narrow", eyes:"closed" })`

b: Ok. Ma io non ho i pollici opponibili, dovrai tracciarla tu.But I've got no opposable thumbs, so you have to do the drawing.

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

h: Nah, hai ragione. One *can* go too far.

`hong({ eyes:"normal" });`

h: Ma ecco perché, con la terapia di esposizione, inizieremo piano piano, a piccoli passi.

h: Prima di andare incontro ai *veri* pericoli, ci fermiamo.

`bb({ eyes:"annoyed_r", mouth:"narrow" });`

b: Yeah I draw the line between hearing loud thunder, and standing in a storm with a tall pointy hat.

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

b: Cosa, nessun commento in merito a come mi sento? Solo... "grazie"?

`hong({ eyes:"surprise", body:"shrug" })`

h: Esatto! Grazie per avermi mostrato la tua preoccupazione per {{_.thanks_for}}.

```
bb({ eyes:"closed_annoyed", MOUTH_LOCK:true });
hong({ eyes:"normal", body:"normal" });
```

b: ...

h: Tutto bene?

`bb({ eyes:"super_sad", mouth:"narrow" });`

b: Non mi avevi mai *ringraziato* prima d'ora.

`hong({ mouth:"smile" });`

h: Oh, il mio lupone pelosone panicone.Aw you big fuzzy-wuzzy panic-wolf.

(#act4_something_else)

# act4_thanks_2

h: Anche se esageri, mi fa piacere che ti preoccupi per {{_.thanks_for}}.

`bb({ eyes:"annoyed" })`

b: Aspetta... Non stai continuando a ringraziarmi solo per evitare di parlare delle paure, vero?

```
bb({ eyes:"normal" });
hong({ eyes:"annoyed", body:"chin" });
```

h: Beh, è complicato, e non ho sempre la risposta a tutto.

`hong({ eyes:"annoyed_l", body:"one_up" })`

h: Nella vita non hai una schermata di dialogo con 3 risposte predefinite.It's not like life gives you a list of 3 pre-made dialogue responses.

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

h: Dai, io una giovane anima vulnerabile e tu un grande lupo spaventoso. Che mai ci può accad-

`hong({ eyes:"normal", body:"point" });`

h: Anzi, meglio non rispondere.

(#act4_something_else)




# act4_alone

```
_.a4_talked_about_alone = true;
_.a4_fears_discussed += 1;
```

`bb({ eyes:"sad_d" });`

b: Voglio solo assicurarmi che tu soddisfi il profondo bisogno umano di appartenenza...

`bb({ eyes:"sad_u" });`

b: Ma ho paura che se mai qualcuno ci dovesse conoscere, *veramente*, li spaventeremmo.

`bb({ eyes:"sad" });`

{{if _.a4_fears_discussed==1}}
b: Non so, enough of *me* choosing what to say next. What do *you* say, human?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: Again, back to you, human. What do you think?
{{/if}}

{{if _.a4_fears_discussed==3}}
b: More thoughts, human?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Sono d'accordo: lavoriamo sulla nostra vita sociale.](#act4_alone_skills)

[Magari piacciamo alle persone. Vogliamo scoprirlo?](#act4_alone_experiment)

[Grazie.](#act4_thanks) `_.thanks_for = "social belonging";`

# act4_alone_skills

```
bb({ eyes:"normal" });
hong({ body:"chin" });
```

h: Potremmo esercitarci su abilità sociali come fare domande, ascoltare, empatizzare, essere aperti e vulnerabili, e così via?We could practice skills like asking questions, listening and empathizing, being open and vulnerable, etc?

`hong({ eyes:"normal_l" });`

h: O migliorare le abitudini sociali, come gestire il tempo con gli amici, o partecipare regolarmente ad incontri?Or make better social habits, like scheduling time with friends or regularly going to meetups?

`hong({ body:"one_up" });`

h: Potremmo anche imparare ad accettare i rifiuti.

`hong({ eyes:"normal" });`

h: O imparare a capire quando le persone *non* ci rifiutano, sono stanchi, o hanno solo la faccia da schiaffi.Or learn to know when people *aren't* rejecting us, they're just tired or have Resting ^Bitch^ Face.

```
hong({ body:"normal" });
bb({ eyes:"annoyed_r" });
```

b: Le opzioni sono tante. Tuttavia, riguardo l'"imparare le abilità sociali"...That's a lot of options. But, about "learning social skills"...

[Non è *manipolazione?*](#act4_alone_skills_manipulative)

[Non ci renderà *più facili da manipolare?*](#act4_alone_skills_manipulated)

[E se non ce la facessimo comunque?](#act4_alone_skills_fail)

# act4_alone_skills_manipulative

`bb({ eyes:"suspect" });`

b: Aren't serial killers who can read their victims' emotions great at "empathy"?

`bb({ eyes:"annoyed" });`

b: Didn't Charles Manson win friends and influence people?

`hong({ eyes:"annoyed", body:"chin" });`

h: No, hai ragione.

h: Le "abilità sociali" non contano nulla se non ci importasse veramente *degli* altri.

`hong({ body:"normal" });`

h: In pratica, non fare gli ^stronzi^.

`bb({ eyes:"annoyed", mouth:"smile" });`

b: Leggi su quel un poster motivazionale.That's a motivational poster caption right there.

`hong({ body:"shrug", mouth:"narrow" });`

h: “Non fare lo ^stronzo^™”

(#act4_something_else)

# act4_alone_skills_manipulated

`bb({ eyes:"angry" })`

b: Diventeremo uno zerbino che dice "per favore" e "grazie" quando le persone ci si puliscono le scarpe sopra, saying Please and Thank You as people wipe their feet on us!

`bb({ mouth:"scream", eyes:"scream" })`

b: Baceremo così tanti ^culi^, che sembrerà che abbiamo messo il rossetto marrone!We'll kiss so much butt, it'll look like we're wearing brown lipstick!

```
bb({ mouth:"normal", eyes:"normal" });
hong( body:"chin" });
```

h: Nah, hai ragione. Le "abilità sociali" non è solo compiacere gli altri, ma anche impostare dei *confini*.  "Social skills" can't be just about pleasing others, it's also got to be about setting *boundaries.*

`hong( body:"one_up" });`

h: Non possiamo invitare persone a casa, se non abbiamo delle mura che la sorreggano.We can't invite others into our home, if we have no walls to hold up our home.

```
hong( eyes:"angry", mouth:"narrow" });
bb( eyes:"annoyed", mouth:"smile" });
```

h: Poi... quella cosa del rossetto... *che schifo*!!Also... re: that lipstick mental image... *ew??*

(#act4_something_else)

# act4_alone_skills_fail

`bb({ eyes:"annoyed" });`

h: Potremmo fallire. Anzi, *falliremo*.

```
bb({ eyes:"normal" });
hong({ eyes:"surprise", body:"shrug" });
```

h: E va bene così! È fallendo che si impara qualcosa di nuovo!Failing is how anyone learns anything new at first!

`hong({ body:"normal", eyes:"normal" });`

h: Quindi falliamo insieme, ok?

`bb({ eyes:"normal_r" });`

b: Immagino di sì... Alle brutte, possiamo cambiare città e farci una nuova identità., we can just skip town and get a new identity.

`bb({ eyes:"normal" });`

h: Sì, forse oggigiorno costa giusto un paio di bitcoin.Yeah I think that only costs two bitcoins these days.

(#act4_something_else)

# act4_alone_experiment

```
hong({ body:"one_up" });
bb({ eyes:"normal" });
```

h: Potremmo provare a sperimentare!We could try some experiments!

`hong({ body:"chin" });`

h: Chiedere a qualche amico di uscire, risentire vecchie conoscenze, oppure chiacchierare con i baristi.We could ping a friend to hang out, reconnect with an old pal, or even just chat with a barista.

`hong({ body:"normal" });`

h: Magari scopriamo di essere più simpatici del previsto.I think we may find we're more likeable than we suspect.

`bb({ eyes:"annoyed" });`

[E se fossero dei piccoli e banali "successi"?What if these are small, cheap "wins"?](#act4_alone_experiment_cheap)

[E se fosse un fardello per gli altri?](#act4_alone_experiment_burden)

[Ma parlare del più e del meno non è *da noi*!](#act4_alone_experiment_real_us)

# act4_alone_experiment_real_us

`bb({ eyes:"sad" });`

b: Se facciamo un finto sorriso, non riusciremo mai a comunicare con nessuno,If we put on a shallow smile, we'll never really connect with anyone,

`bb({ eyes:"super_sad" });`

b: *Ma* se ci apriamo, gli altri vedranno tutto il nostro disordine interno!*But* if we open up, other people will see all our messed-up insides!

`hong({body:"chin", mouth:"narrow", MOUTH_LOCK:true})`

h: ...

```
hong({body:"normal", mouth:"normal"});
bb({eyes:"normal"});
```

h: Rotola.

b: Cosa.

`hong({body:"hands_1"})`

h: Quando i cani vogliono esprimere amore e fiducia, si rendono vulnerabili mostrando la pancia.When dogs want to show love and trust, they make themselves vulnerable by exposing their belly.

`hong({body:"one_up"})`

h: Forse non siamo *ancora* abbastanza al sicuro per essere troppo vulnerabili, ma esercitandoci,Maybe we're not *yet* secure enough to be too vulnerable, but with enough training,

`hong({body:"normal", eyes:"surprise"})`

h: Un giorno riusciremo a mostrarci per quello che siamo: disastrati, ma umani.One day we can show people the real us – all messed-up, all human.

```
hong({eyes:"normal"});
bb({ eyes:"super_sad", mouth:"smile", body:"chest" });
```

b: Rotolerò solo se mi dai un biscottino.I'll roll over if you give me a treat.

`bb({ eyes:"normal", mouth:"normal" });`

h: No.

(#act4_something_else)


# act4_alone_experiment_cheap

b: Dire "ciao" ai baristi non è proprio una prestazione da medaglia d'oro alle Socialimpiadi.Saying "hi" to the barista isn't exactly gold-medal performance in the Social Butterfly Olympics.

```
hong({ body:"point", eyes:"surprise" });
bb({ eyes:"normal" });
```

h: Lo è per *noi*!

`hong({ body:"one_up", eyes:"annoyed" });`

h: Nel ring sociale, non siamo nemmeno peso piuma, siamo tipo... peso ricotta.

`hong({ body:"normal", eyes:"normal" });`

h: Se dobbiamo iniziare con piccoli e banali successi, facciamolo. Per arrivare al millesimo gradino, dobbiamo prima salire sul primo.If we have to start with small, cheap wins, so be it. Gotta climb the 1st step before the 1000th step.

b: Esatto! Magari dopo aver detto "ciao", possiamo proseguire dicendo...Yeah! Maybe after saying "Hi", we can advance to saying...

`bb({ body:"two_up", mouth:"smile", eyes:"smile_u" });`

b: *"Come stai?"*

`hong({ body:"shrug", mouth:"smile", eyes:"surprise_l" });`

h: *"Non c'è male!*

(#act4_something_else)

# act4_alone_experiment_burden

`bb({ eyes:"suspect_r" })`

b: Forse vuole solo fare un dannato caffè, non diventare una *cavia* dei nostri fallimenti nelle interazioni sociali.Maybe the barista just wants to make some dang coffee, not be an *experiment* to see if our social skills suck.

`bb({ eyes:"annoyed" })`

h: Beh, se ci riveliamo *essere* un fardello...Well, if it turns out we *are* being a burden...

```
hong({ eyes:"surprise" });
bb({ eyes:"normal" });
```

h: Comunque buon per noi!That's good to know, too!

`hong({ eyes:"normal" });`

h: Possiamo imparare a chiedere proattivamente agli altri cosa li mette a proprio agio, per conoscere e rispettare i confini altrui. We can then learn how to pro-actively ask people what they're comfortable with, to know and respect others' boundaries.

```
hong({ eyes:"annoyed_l", mouth:"narrow" });
bb({ eyes:"annoyed", mouth:"smile" });
```

h: Sai, tutta quella robaccia delle "abilità interpersonali" che vediamo sui volantini del consulente.Y'know, all that "inter-personal skills" ^crap^ we see in counselor brochures.

(#act4_something_else)



# act4_bad

```
_.a4_talked_about_bad = true;
_.a4_fears_discussed += 1;
```

`bb({ eyes:"annoyed_r" })`

b: Voglio difendere i tuoi bisogni morali, che ti portano a diventare una persona migliore,I want to defend your moral needs, that drive to become a better person,

`bb({ eyes:"sad_d" })`

b: Ma sembra che, in fondo, siamo completamente... rotti.But it just feels like deep down, we're so fundamentally... broken.

`bb({ body:"two_up", eyes:"angry" })`

{{if _.INJURED}}
b: E non dirmi che *non* siamo incasinati. Siamo saltati da un *tetto*.And don't tell me we're *not* messed up. We jumped off a *roof*.
{{/if}}

{{if !_.INJURED}}
b: E non dirmi che *non* siamo incasinati. Siamo quasi saltati da un *tetto*.
{{/if}}

`bb({ body:"normal", eyes:"sad" })`

{{if _.a4_fears_discussed==1}}
b: I dunno, enough of *me* choosing what to say next. What do *you* say, human?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: Again, back to you, human. What do you think?
{{/if}}

{{if _.a4_fears_discussed==3}}
b: More thoughts, human?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Dunque siamo rotti. Rimediamo.](#act4_bad_fix)

[Dunque, siamo rotti. Accettiamolo.](#act4_bad_accept)

[Grazie.](#act4_thanks) `_.thanks_for = "moral well-being";`

# act4_bad_fix

```
bb({eyes:"normal"});
hong({body:"chin"});
```

h: Potremmo piano piano acquisire abitudini più sane, e rendere la nostra vita più in linea con i nostri valori,We could slowly build better habits, get our life more in line with what we value,

`hong({body:"one_up"});`

h: E, se necessario, potremmo chiedere un aiuto professionale: uno psicologo o un consulente.And if needed, we could get professional help – a therapist or counsellor.

`hong({body:"normal"});`

h: I modi per uscirne ci sono.There's ways to fix us.

[E se non riuscissimo a uscirne del tutto?What if we can't fix it all?](#act4_bad_fix_cant)

[E se ne uscissimo *fin* troppo?What if we fix *too* much?](#act4_bad_fix_too_much)

[Non possiamo permetterci un aiuto professionale.](#act4_bad_fix_afford)

# act4_bad_fix_cant

`hong({eyes:"annoyed"});`

h: Nah, I guess you're right.

h: Non possiamo uscirne del tutto.We can't fix it all.

`bb({mouth:"scream", eyes:"scream_sad"});`

b: Ahhh lo sapevo che saremo sempre rotti! I knew it we'll always be broken!

`hong({eyes:"surprise"});`

h: Ma possiamo almeno essere *meno* rotti.But we can at least be *less* broken.

```
bb({mouth:"normal", eyes:"annoyed"});
hong({eyes:"sad", mouth:"smile"});
```

h: Le cicatrici si curano col tempo, ma non se ne andranno più. E va bene così. Scars heal with time, but they never go away. And that's okay.

`bb({eyes:"annoyed_r"});`

b: Credo di sì. Inoltre,

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

h: Ti prego, no.Please do not do that.

(#act4_something_else)

# act4_bad_fix_too_much

`bb({ eyes:"angry_d" })`

b: Fa schifo ammetterlo, ma... una parte di me *vuole* avere questo disordine.This feels sick to admit, but... some part of me *wants* to have this disorder.

`bb({ eyes:"angry" })`

b: Voglio dire, non è che siamo *noiosi* senza?I mean, without it, won't we be *boring?*

`bb({ eyes:"sad_r", body:"one_up" })`

b: Senza il disordine, la nostra arte non è che diventa Without the disorder, won't our art become stale and bland?

`bb({ eyes:"sad_u", body:"two_up" })`

b: Senza il disordine, won't we be unable to connect with our friends who have the disorder?

`bb({ eyes:"sad", body:"chest" })`

b: Se saremo mai soddisfatti nella vita, If we're ever content with life, won't we stop driving ourselves to do great things?

`hong({ MOUTH_LOCK:true })`

h: ...

h: If we even fear... "running out of fears"...

h: I don't think we're gonna run out of fears.

`bb({ eyes:"smile_u", body:"normal", mouth:"smile" })`

b: Oh, sì! Uh, che sollievo!

(#act4_something_else)

# act4_bad_fix_afford

`bb({ body:"one_up", eyes:"sexy", mouth:"normal" })`

b: "Doc, I'm anxious that I'm paying $100/hr just to hear you ask *how does that make you feel?*"

`bb({ body:"paw", eyes:"closed", mouth:"narrow" })`

b: "Mm-hmm. E questo come ti fa sentire?"

```
bb({ body:"normal", eyes:"normal", mouth:"normal" });
hong({ eyes:"sad" });
```

h: Nah, è una preoccupazione piuttosto ragionevole.Nah, that's a totally reasonable worry.

`hong({ eyes:"annoyed", mouth:"sad" });`

h: E fa veramente schifo che la sanità mentale è un lusso per tanta gente.And it genuinely sucks that mental healthcare isn't affordable for lots of folks.

`hong({ eyes:"normal", mouth:"normal" });`

h: Ma ci sono anche opzioni economiche o gratuite:

`hong({ body:"chin" })`

h: Gruppi di supporto, terapia online, student/non-profit health centers...

`hong({ body:"hands_1" })`

h: Building habits like meditation, sleeping well, chatting regularly with friends, learning new things...

`hong({ body:"hands_2" })`

h: Andare in biblioteca e prendere in prestito workbooks for evidence-based psychotherapies...

`hong({ body:"one_up" })`

h: Alla fine c'è una lunga lista di risorse!

```
hong({ body:"normal" });
bb({ eyes:"annoyed", mouth:"narrow" });
```

b: Beh, *quella* quarta parete non è durata molto.

`hong({ body:"point" });`

h: Ci sono cose più importanti delle regole di narrazione. Come la salute mentale.Some things are more important than narrative convention. Such as mental health.

(#act4_something_else)


# act4_bad_accept

```
bb({ eyes:"normal" });
hong({ eyes:"normal_l", body:"one_up", mouth:"narrow" });
```

h: Insomma, è quello che dicono gli psicologi, no? Accettare i tuoi sentimenti, anche quelli negativi?I mean, that's what therapists say right? Accept all your emotions, even the negative ones?

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

b: Pensi che Martin Luther King avrebbe detto: "Shucks we can't sit in the front of the bus, let's just *accept* it?"

`bb({ eyes:"angry_r", body:"two_up" });`

b: Why does the Self-Help Industrial Complex think waving the white flag is some *profound wisdom?*

`bb({ eyes:"annoyed", body:"normal" });`

h: I think therapists mean "accept" bad things as in: acknowledging they exist and are hard to change,

h: But not necessarily giving up a commitment to change.

`bb({ eyes:"suspect" });`

b: Allora gli psicologi dovrebbero dire *riconoscere*, non *accettare*.

`hong({ body:"chin", eyes:"annoyed" });`

h: Pensaci, *accettare* è abbastanza fuorviante.Yeah come to think of it, "accept" is kinda confusing.

`bb({ eyes:"closed", mouth:"narrow" });`

b: Beh, lo *riconosco*.

(#act4_something_else)

# act4_bad_accept_approve

`bb({ eyes:"angry" });`

b: Like it's *good* that we're broken or something? No!

`bb({ eyes:"angry_r", body:"one_up" });`

b: All those dang Hollywood screenwriters who romanticize mental illness are full of crud!

`bb({ eyes:"angry", body:"two_up" });`

b: Avere un disturbo mentale *fa schifo*! Deruba le persone della *vita*! Perché dovremmo *accettarlo*?Having a mental disorder *sucks!* It robs people of *lives!* Why should we "accept" that?!

`bb({ body:"normal" });`

h: Penso che gli psicologi intendano "accettare" le nostre emozioni nel senso di essere pazienti con esse.I think therapists mean "accept" our emotions as in: be patient with them.

```
hong({ body:"one_up" });
bb({ eyes:"normal" });
```

h: Like how struggling in quicksand makes you sink faster, and the solution is to patiently lie flat,

`hong({ eyes:"surprise" });`

{{if _.INJURED}}
h: Fighting against you, my fear, led me to jump off a roof.
{{/if}}

{{if !_.INJURED}}
h: Fighting against you, my fear, almost led me to jump off a roof.
{{/if}}

`hong({ body:"normal", eyes:"normal" });`

h: Instead, the solution is to do what we're doing now – not to fight, but to patiently be with each other.

`bb({ eyes:"annoyed" });`

b: Then they should say *that* instead of some problematic word like "accept".

`hong({ body:"chin", eyes:"annoyed" });`

h: Yeah come to think of it, "accept" kind of sucks.

`bb({ eyes:"closed_annoyed", mouth:"narrow" });`

b: I do not accept "accept".

(#act4_something_else)

# act4_bad_accept_literally

`bb({ eyes:"sad", body:"one_up" });`

b: But we already *know* you shouldn't take me literally!

`bb({ eyes:"sad_u", body:"two_up" });`

b: The whole *problem* is that I want to help you, but I suck at using words to do so!

`bb({ eyes:"sad", body:"normal" });`

h: I think therapists mean "accept" your emotions as in: "don't fight or ignore them."

`hong({ eyes:"surprise", body:"one_up" });`

h: To listen to you, work *with* you, but not take what you say as 100% literal truth.

```
hong({ eyes:"normal", body:"normal" });
bb({ eyes:"annoyed", mouth:"normal" });`
```

b: Then therapists should say *that* instead of some vague confusing word like "accept".

`hong({ body:"chin", eyes:"annoyed" });`

h: I guess they suck at using words, too.

(#act4_something_else)




# act4_something_else

```
bb({ body:"normal", mouth:"normal", eyes:"normal" });
hong({ body:"normal", mouth:"normal", eyes:"normal" });
```

{{if _.a4_fears_discussed==1}}
h: Anyway, anything else you wanna chat about?
{{/if}}

{{if _.a4_fears_discussed==2}}
h: So, anything else on your heavy heart?
{{/if}}

{{if _.a4_fears_discussed==3}}
(#act4_something_else_2)
{{/if}}

{{if _.a4_talked_about_harm!=true}}
[I'm scared we'll be harmed.](#act4_harm)
{{/if}}

{{if _.a4_talked_about_alone!=true}}
[I'm scared we'll be alone.](#act4_alone)
{{/if}}

{{if _.a4_talked_about_bad!=true}}
[I'm scared we're bad people.](#act4_bad)
{{/if}}

[Nah, I'm good for now.](#act4c_prelude)

# act4_something_else_2

h: Okay, I think we've talked about all our fears now.

b: Yes, there are only three fears.

h: Yup, exactly three.

b: Convenient.

(#act4c)

# act4c_prelude

h: Good chat, team.

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

b: This isn't some *game*, you know.

`bb({eyes:"angry_d", body:"one_up"})`

b: Building a healthy relationship with your emotions isn't as simple as clicking buttons on a screen.

`bb({eyes:"sad", body:"normal"})`

b: *Can* we really get along?

b: *Can* we work together, as a team?

`hong({eyes:"sad", body:"one_up"})`

h: Well,

```
hong({eyes:"surprise_l"});
bb({eyes:"normal"});
```

a: E-excuse me...

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

a: W-wo-would you mind if I sat with you for lunch?

`publish("act4", ["alshire", 1]);`

{{if _.TOP_FEAR=="harm"}}
s: *This* is your crush? Why are they sitting alone like a psycho serial killer?
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: Asking your crush if you can sit with them? Do you know how *needy* we sound?!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: *This* is your crush? We interrupted their peace and quiet! We're such a burden!
{{/if}}

`publish("act4", ["alshire", 2]);`

a: I- I mean- it's, it's okay if not, I just...

`publish("act4", ["alshire", 3]);`

`Game.OVERRIDE_CHOICE_SPEAKER = "h2"`

[Wait, didn't I see you at the party?](#act4d_recognition) `publish("act4", ["hong_to_alshire",1])`

[Yeah, of course! Come here.](#act4d_yes) `publish("act4", ["hong_to_alshire",2])`

[Sorry, I need alone time right now.](#act4d_no) `publish("act4", ["hong_to_alshire",8])`

# act4d_recognition

`publish("act4", ["hong_to_alshire",2]);`

h2: Yeah you were on the couch! At the first party I went to...

`publish("act4", ["hong_to_alshire",10]);`

{{if _.a2_ending=="fight"}}
h2: Where I had that panic attack and punched the host.
{{/if}}

{{if _.a2_ending=="flight"}}
h2: Where I had that panic attack and ran out crying.
{{/if}}

```
publish("act4", ["hong_to_alshire", 0]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: Hang on human, we may be making them uncomfortable.

```
publish("act4", ["hong_to_alshire", 3]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: Ah, I don't mean to put you on the spot!

`publish("act4", ["hong_to_alshire",4]);`

h2: Just remembering a friendly face, is all.

```
publish("act4", ["hong_to_alshire",5]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: AHHHHH I KNEW IT! THEY'RE A DANGEROUS PANIC-DRIVEN PSYCHO!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: AAHHH THE FIRST IMPRESSION WE MADE WAS "WITNESSED MY TRAUMA"! THAT MEANS THEY HATE US!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: AAAHHH WE MADE SOMEONE REMEMBER A TRAUMATIC EVENT. OUR MERE PRESENCE HURTS OTHERS.
{{/if}}

(#act4e)

# act4d_yes

```
publish("act4", ["hong_to_alshire", 5]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: Hang on human, they seem uncomfortable.

```
publish("act4", ["hong_to_alshire", 6]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: Ah, no pressure of course!

`publish("act4", ["hong_to_alshire", 4]);`

h2: Just saying, you can sit here if you want to.

```
publish("act4", ["hong_to_alshire", 5]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: THEY'RE BEING *TOO* FRIENDLY! LIKE TED BUNDY, THE SERIAL KILLER!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: THEY'RE JUST ACTING NICE! NO ONE *REALLY* WANTS TO BE CLOSE TO US!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: AHHH WE ALWAYS MAKE OTHERS FEEL AWKWARD! WE'RE A STAIN UPON THE EARTH!
{{/if}}

(#act4e)

# act4d_no

```
publish("act4", ["hong_to_alshire", 9]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: Hang on human, we may be making them uncomfortable.

```
publish("act4", ["hong_to_alshire", 3]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: Ah, I don't mean to be rude!

`publish("act4", ["hong_to_alshire", 6]);`

h2: I just need some time to process my emotions. Please don't take it as a personal rejection.

```
publish("act4", ["hong_to_alshire", 7]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: WHAT SICK, TWISTED THOUGHTS ARE THEY PROCESSING?! WHAT DARK DESIRES FILL THIS PSYCHO'S HEART?!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: WE'VE BEEN PERSONALLY REJECTED! WE'LL NEVER BE LOVED!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: WE INTERRUPTED THEIR EMOTIONAL PROCESSING! NOW THEY'LL BE TRAUMATIZED FOREVER AND IT'S ALL OUR FAULT!
{{/if}}

(#act4e)

# act4e

```
Game.WORDS_HEIGHT_BOTTOM = 195;
publish("act4", ["alshire", 6]);
```

s: RUN RUN RUN RUN RUN RUN RUN RUN RUN RUN RUN RUN RUN RUN RUN

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

h: Huh. That was weird. I wonder what was going on in their head.

`publish("act4", ["hong_closer", 2]);`

h: Anyway, you were saying?

```
publish("act4", ["hong_closer", 1]);
publish("act4", ["bb_closer", 6]);
```

b: Uh, I forget? Something about teams and work?

```
publish("act4", ["bb_closer", 0]);
publish("act4", ["hong_closer", 3]);
```

h: ¯\_(ツ)_/¯

```
publish("act4", ["hong_closer", 1]);
publish("act4", ["bb_closer", 4]);
```

b: They say you should "make peace" with your emotions, as if your emotions are *war criminals*.

`publish("act4", ["bb_closer", 7]);`

b: But I want us to make *more* than mere peace! I want us to be *allies!*

`publish("act4", ["bb_closer", 3]);`

b: I want to be a good guard-dog. Just like how hunger & thirst are alarms for your physical needs,

`publish("act4", ["bb_closer", 8]);`

b: I want to be the alarm for your *psychological* needs – your needs for safety, belonging, goodness.

`publish("act4", ["bb_closer", 1]);`

b: But... I suck at my job, so I need you to train me.

`publish("act4", ["bb_closer", 4]);`

b: I'm not "always valid," nor "always irrational." I'm just... trying my best. So, please,

`publish("act4", ["bb_closer", 30]);`

b: Help me help you!

`publish("act4", ["bb_closer", 6]);`

b: Though, teaching an old dog new tricks *will* take a while. Maybe *years.*

`publish("act4", ["bb_closer", 3]);`

b: And sometimes I'll relapse, I'll slip into my old habits.

`publish("act4", ["bb_closer", 2]);`

b: I'll bark at shadows. I'll scare you with words. I might even show you some intrusive images of... things.

`publish("act4", ["bb_closer", 9]);`

b: I'm sorry! I'm a battered shelter dog! Battered dogs poop on your bed sometimes!

`publish("act4", ["bb_closer", 4]);`

b: But if you're patient with me... and just stay and sit with me...

`publish("act4", ["bb_closer", 8]);`

b: Maybe you can tame this wolf.

`publish("act4", ["bb_closer", 0]);`

`Game.clearText();`

(...1000)

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Good dog.](#act4f-pat-bb) `Game.OVERRIDE_CHOICE_SPEAKER = "h"; publish("act4", ["hong_closer", 2]);`

`Game.OVERRIDE_CHOICE_SPEAKER = "b"`

[Good human.](#act4f-pat-hong) `Game.OVERRIDE_CHOICE_SPEAKER = "b"; publish("act4", ["bb_closer", 8]);`

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
b: AAAAA YOU'RE STILL EATING ALONE FIFTEEN CIGARETTES AAAAA
{{/if}}

{{if _.parasite}}
b: AAAAA YOU'RE STILL NOT PRODUCTIVE WHILE EATING WE'RE SOCIETY-PARASITES AAAAA
{{/if}}

{{if _.whitebread}}
b: AAAAA YOU'RE EATING MORE WHITE BREAD AAAAA
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

b: YAP YAP YAP YAP YAP

(#credits)
