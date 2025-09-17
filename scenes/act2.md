# act2

`SceneSetup.act2();`

{{if _.badnews && !_.factcheck}}
(#act2-preamble-news1)
{{/if}}

{{if _.badnews && _.factcheck}}
(#act2-preamble-news2)
{{/if}}

{{if _.catmilk}}
(#act2-preamble-cat)
{{/if}}

(#act2-preamble-tinder)


# act2-preamble-news1

```
publish("act2",["dee",3]);
```

s: Ma hai *letto* la "notizia" di quel fattaccio orribile successo non so dove?

```
publish("act2",["dee",2]);
publish("act2",["party_hong","next"]);
```

h2: C-ciao...

```
publish("act2",["party_hunter",1]);
publish("act2",["party_hong","next"]);
publish("act2",["dum",3]);
```

a: Dio, odio quei post. Tutto sensazionalismo per farti cliccare.

```
publish("act2",["dum",2]);
publish("act2",["party_hong","next"]);
```

h2: B... bella festa...

```
publish("act2",["party_hong","next"]);
publish("act2",["party_hunter",0]);
publish("act2",["dee",1]);
```

s: Vero, ma lo fanno solo per incentivare. Il *vero* problema è chi ci clicca.

```
publish("act2",["dee",3]);
```

s: Chi mai retwitterebbe una notizia così terribile e far star male i suoi amici?

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Ah, puoi dirlo forte!

(#act2-preamble-end)


# act2-preamble-news2

```
publish("act2",["dee",3]);
```

s: Ma hai *letto* quella "notizia" andata virale?

```
publish("act2",["dee",2]);
publish("act2",["party_hong","next"]);
```

h2: C-ciao...

```
publish("act2",["party_hunter",1]);
publish("act2",["party_hong","next"]);
publish("act2",["dum",3]);
```

a: Sì, palesemente una bufala. Chi ci crederebbe mai da retwittarla?

```
publish("act2",["dum",2]);
publish("act2",["party_hong","next"]);
```

h2: B... bella festa...

```
publish("act2",["party_hong","next"]);
publish("act2",["party_hunter",0]);
publish("act2",["dee",3]);
```

s: Ma sul serio. Cioè, tutto ok? Andare su Google a verificare prima?

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Ah, puoi dirlo forte!

(#act2-preamble-end)


# act2-preamble-cat

```
publish("act2",["dee",3]);
```

s: Come dicevo, il Complesso Industriale dei Meme sfrutta i gatti.

```
publish("act2",["dee",2]);
publish("act2",["party_hong","next"]);
```

h2: C-ciao...

```
publish("act2",["party_hunter",1]);
publish("act2",["party_hong","next"]);
publish("act2",["dum",1]);
```

a: Elabora la tua tesi.

```
publish("act2",["dum",0]);
publish("act2",["party_hong","next"]);
```

h2: B... bella festa...

```
publish("act2",["party_hong","next"]);
publish("act2",["party_hunter",0]);
publish("act2",["dee",1]);
```

s: Beh, ieri qualcuno ha retwittato una GIF di un gatto che beve il latte.

```
publish("act2",["dee",3]);
```

s: Ma non lo digeriscono! Chi mai retwitterebbe un *abuso sugli animali* del genere?

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Ah, puoi dirlo forte!

(#act2-preamble-end)


# act2-preamble-tinder

```
publish("act2",["dee",1]);
```

s: E quindi non ha mai risposto!

```
publish("act2",["dee",0]);
publish("act2",["party_hong","next"]);
```

h2: C-ciao...

```
publish("act2",["party_hunter",1]);
publish("act2",["party_hong","next"]);
publish("act2",["dum",1]);
```

a: Anche se avete matchato su Tinder?

```
publish("act2",["dum",0]);
publish("act2",["party_hong","next"]);
```

h2: B... bella festa...

```
publish("act2",["party_hong","next"]);
```

{{if _.serialkiller}}
(#act2-preamble-serialkiller)
{{/if}}

{{if _.hookuphole}}
(#act2-preamble-hookuphole)
{{/if}}

{{if _.pokemon}}
(#act2-preamble-pokemon)
{{/if}}

# act2-preamble-serialkiller

```
publish("act2",["party_hunter",0]);
publish("act2",["dee",3]);
```

s: Ma che ne so! Pensa forse che sia un *serial killer* o cosa? Quante paranoie.

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Ah, puoi dirlo forte!

(#act2-preamble-end)


# act2-preamble-hookuphole

```
publish("act2",["party_hunter",0]);
publish("act2",["dee",3]);
```

s: Ma che ne so! Pensa che gli incontri non possano colmare il vuoto nel suo cuore?

s: Quanto sei moralista! Apri la mente, e poi le gambe!

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Ah, puoi dirlo forte!

(#act2-preamble-end)


# act2-preamble-pokemon

```
publish("act2",["party_hunter",0]);
publish("act2",["dee",3]);
```

s: Ma che ne so! Non era un granché, ma poteva essere un bell'acchiappo!

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Acchiappali tutti!™

(#act2-preamble-end)


# act2-preamble-end

```
Game.clearText();
publish("act2-out-1");
music(null, {fade:1});
```

(...3000)

```
music('battle', {volume:0.5});
publish("hp_show");
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

n: ROUND TWO: *FIGHT!*

[Oh no, ci odiano tutti!](#act2a_social)

[Stavi *adocchiando* "Pel di carota"?](#act2a_perv)

[Ehi, parliamo del senso della vita.](#act2a_meaning)

# act2a_social

`bb({eyes:"sad"})`

b: Stiamo rovinando il clima della festa facendo i musoni!

`bb({eyes:"shock", body:"two_up"})`

b: Stiamo uccidendo l'atmosfera! Stiamo commettendo un atmosfericidio di primo grado!

`bb({eyes:"normal", body:"normal"})`

b: Dobbiamo andarcene *ora*, prima che-

```
_.a2_first_danger = 'social';
_.a2_attack_1 = "alone";
```

(#act2b)

# act2a_perv

`bb({eyes:"suspect"})`

b: È più attraente di noi, vuol dire che se ci mettiamo a *fissare*, allora-

`bb({eyes:"shock", body:"two_up"})`

b: SIAMO DEI MANIACI

`bb({body:"normal"})`

b: Siamo dei viscidi, orribili, brutti e cattivi perv-

```
_.a2_first_danger = 'perv';
_.a2_attack_1 = "bad";
```

(#act2b)

# act2a_meaning

`bb({body:"one_up", eyes:"normal_r"})`

b: In fin dei conti, cosa possiamo fare di così rilevante?

`bb({body:"normal", eyes:"sad"})`

b: Contribuire all'umanità? Le grandi opere subiscono la sorte di Osimandia. Amare? La morte ha l'ultima parola.

`bb({eyes:"sad_r"})`

b: E di morte ce n'è un sacco! *Noi* moriremo. *I nostri cari* moriranno.

`bb({eyes:"shock", body:"two_up"})`

b: Cioè, la 2ª Legge della Termodinamica dimostra che anche il nostro *universo* morirà!

`bb({eyes:"suspect", body:"normal"})`

b: Oh, "la morte ci fa apprezzare la vita"? È come dire che la schiavitù è bella perché ci fa apprezzare la libertà!

`bb({body:"one_up"})`

b: Oh, "dai un senso alla tua esistenza"? È quello che fanno i cultisti e i cospirazionisti!

`bb({eyes:"shock", body:"two_up"})`

b: La vita non ha senso, la morte non ha senso, neanche il *senso* ha senso! Che dovrebbe fare un'anima mortale-

```
_.a2_first_danger = 'meaning';
_.a2_attack_1 = "bad";
```

(#act2b)

# act2b

`bb({eyes:"normal", mouth:"normal", body:"normal", MOUTH_LOCK:true})`

b: ...

`bb({eyes:"suspect"})`

b: Ehm... mi senti?

`bb({eyes:"normal", MOUTH_LOCK:true})`

b: ...

`bb({eyes:"shock", mouth:"small_talk", body:"chest", MOUTH_LOCK:true})`

b: *AHHH*

`bb({mouth:"small_talk"})`

b: DEVO AVVERTIRTI DI...

[*Altri pericoli* dello stesso pericolo!](#act2b_louder)

{{if _.a2_first_danger=="social"}}
[Un *nuovo* pericolo sociale!](#act2b_different_social)
{{/if}}

{{if _.a2_first_danger=="perv" || _.a2_first_danger=="meaning"}}
[Un *nuovo* pericolo morale!](#act2b_different_moral)
{{/if}}

[Non ignorare il pericolo! È pericoloso!](#act2b_ignore)

# act2b_louder

`_.a2_first_choice = "louder"`

{{if _.a2_first_danger=="social"}}
(#act2b_louder_social)
{{/if}}

{{if _.a2_first_danger=="perv"}}
(#act2b_louder_perv)
{{/if}}

{{if _.a2_first_danger=="meaning"}}
(#act2b_louder_meaning)
{{/if}}

# act2b_louder_social

`bb({eyes:"shock", body:"two_up", mouth:"normal"})`

b: LE EMOZIONI SONO CONTAGIOSE! E SE NON TE NE VAI, INFETTERAI TUTTI CON LA TUA MALATTIA MENTALE!

b: Creerai un'epidemia mortale della SINDROME DEL MUSONE

`bb({eyes:"suspect", body:"normal", mouth:"normal"})`

b: Dobbiamo andarcene e metterci per sempre in quarantena in una stanzetta con Netflix e cibo d'asporto!

```
_.a2_second_danger = 'netflix';
_.a2_attack_2 = "alone";
_.a2_hoodie_callback = "a quarantine";
```

(#act2c)

# act2b_louder_perv

`bb({eyes:"suspect", body:"two_up", mouth:"normal"})`

b: NON FARE IL VERME. È CONTRO LA LEGGE!

`bb({eyes:"judge", body:"judge_1", mouth:"normal"})`

(...201)

```
bb({body:"judge_2"}, 0);
sfx("gravel");
```

(...168)

`bb({body:"judge_1"}, 0)`

(...168)

`bb({body:"judge_2"}, 0)`

(...168)

`bb({body:"judge_1"}, 0)`

(...501)

b: Legge del Verme, Sezione 74.5: (1) Chiunque fissi (a) quelle spalle muscolose (b) quel sedere spumeggiante (2) sarà considerato

`bb({eyes:"shock", body:"two_up", mouth:"normal"})`

b: "UN ENORME, DISGUSTOSO, SCHIFOSO VERME"

```
_.a2_second_danger = 'law';
_.a2_attack_2 = "bad";
_.a2_hoodie_callback = "the law";
```

(#act2c)

# act2b_louder_meaning

`bb({body:"two_up", mouth:"normal", eyes:"shock"})`

b: In realtà, anche se trovassi un valido scopo nella vita, potresti *sempre* rovinare tutto!

`bb({body:"normal", mouth:"normal", eyes:"normal"})`

b: Alfred Nobel voleva la pace nel mondo e che le culture socializzassero. Quindi, ha deciso di semplificare i viaggi.

`bb({eyes:"normal_r"})`

b: Gli serviva un modo economico per creare i tunnel per i treni, così inventò un materiale chiamato "dinamite"...

`bb({body:"one_up", eyes:"normal"})`

b: Utilizzata nella I Guerra Mondiale per UCCIDERE MILIONI DI PERSONE

`bb({body:"two_up", eyes:"shock"})`

b: È L'EFFETTO FARFALLA! STAI INCOSAPEVOLMENTE UCCIDENDO UN SACCO DI PERSONE IN QUESTO MOMENTO

```
_.a2_second_danger = 'butterfly';
_.a2_attack_2 = "bad";
_.a2_hoodie_callback = "World War I";
```

(#act2c)

# act2b_different_social

`_.a2_first_choice = "different"`

`bb({eyes:"normal_r", body:"point", mouth:"normal"})`

b: Sai in realtà cos'è peggio di non essere amati da nessuno? Essere amati da tutti.

`bb({body:"one_up", eyes:"suspect", mouth:"normal"})`

b: E diventare come *questi* animali da festa a caccia di piaceri.

`bb({body:"normal", mouth:"small"})`

b: Una vita frivola con amici frivoli che conoscono solo il tuo lato frivolo!

`bb({body:"two_up", eyes:"shock", mouth:"normal"})`

b: Dobbiamo scappare da questi zombie del piacere, prima che ci facciano diventare come loro!

```
_.a2_second_danger = 'zombies';
_.a2_attack_2 = "alone";
_.a2_hoodie_callback = "zombies";
```

(#act2c)

# act2b_different_moral

`_.a2_first_choice = "different"`

`bb({body:"two_up", eyes:"shock", mouth:"normal"})`

b: *Proprio ora* c'è chi muore di carestie e genocidi, e noi stiamo facendo festa!

`bb({body:"point", eyes:"closed", mouth:"small"})`

b: Un saggio disse, "l'unica cosa necessaria per far sì che il male trionfi è che i buoni non facciano nulla".

`bb({body:"two_up", eyes:"shock", mouth:"normal"})`

b: NON STIAMO FACENDO NULLA.

`bb({mouth:"small"})`

b: FACENDO FESTA, STIAMO AIUTANDO *HITLER*.

```
_.a2_second_danger = 'hitler';
_.a2_attack_2 = "bad";
_.a2_hoodie_callback = "Hitler";
```

(#act2c)

# act2b_ignore

`_.a2_first_choice = "ignore"`

`bb({body:"normal", mouth:"normal", eyes:"suspect"})`

b: Pensi di essere al sicuro solo togliendo le batterie dal rilevatore di monossido di carbonio?

`bb({eyes:"suspect_r"})`

b: Non riuscirai nemmeno a sentirne l'odore! Ti addormenterai e poi-

`bb({body:"scream_c_1"})`

b: MORIRAIIIIIIIIIIIIII

```
_.a2_second_danger = 'ignore';
_.a2_attack_2 = "harm";
_.a2_hoodie_callback = "carbon monoxide";
```

(#act2c)

# act2c

```
hong({body:"ignore_sweat"});
bb({eyes:"normal", mouth:"normal", body:"normal", MOUTH_LOCK:true});
```

b: ...

`bb({eyes:"happy", mouth:"smile", body:"chest"})`

b: Oh, grazie al cielo, forse riesci di nuovo a sentirmi!

`bb({eyes:"closed", body:"point"})`

b: DEVO AVVISARTI DI...

{{if _.a2_first_choice=="louder"}}
[*Ancora altri* pericoli dello stesso pericolo!](#act2c_louder)
{{/if}}

{{if _.a2_first_choice!="louder"}}
[*Altri pericoli* dello stesso pericolo!](#act2c_louder)
{{/if}}

{{if _.a2_first_danger=="social"}}
[Un *nuovo* pericolo sociale!](#act2c_different_social)
{{/if}}

{{if _.a2_first_danger=="perv" || _.a2_first_danger=="meaning"}}
[Un *nuovo* pericolo morale!](#act2c_different_moral)
{{/if}}

[Hai controllato il drink prima di berlo?](#act2c_punch)

#act2c_louder

{{if _.a2_second_danger=="netflix"}}
(#act2c_louder_netflix)
{{/if}}

{{if _.a2_second_danger=="law"}}
(#act2c_louder_law)
{{/if}}

{{if _.a2_second_danger=="butterfly"}}
(#act2c_louder_butterfly)
{{/if}}

{{if _.a2_second_danger=="zombies"}}
(#act2c_louder_zombies)
{{/if}}

{{if _.a2_second_danger=="hitler"}}
(#act2c_louder_hitler)
{{/if}}

{{if _.a2_second_danger=="ignore"}}
(#act2c_louder_ignore)
{{/if}}

# act2c_louder_netflix

`bb({body:"normal", mouth:"normal", eyes:"shock"})`

b: Forse l'idea "Netflix e cibo d'asporto" non è abbastanza sicura! Potremmo comunque infettare il corriere!

`bb({body:"one_up", mouth:"small"})`

b: Dobbiamo trasferirci nell'area canadese dello Yukon, e farci spedire il cibo dai droni!

`bb({body:"two_up", mouth:"normal"})`

b: E dovranno sterilizzare il drone per eliminare i GERMI DEL MUSONE

`_.a2_attack_3 = "alone";`

`_.a2_hoodie_callback = "a quarantine";`

(#act2d)

# act2c_louder_law

`bb({eyes:"judge", body:"judge_1", mouth:"normal"})`

(...201)

```
bb({body:"judge_2"}, 0);
sfx("gravel");
```

(...168)

`bb({body:"judge_1"}, 0)`

(...168)

`bb({body:"judge_2"}, 0)`

(...168)

`bb({body:"judge_1"}, 0)`

(...501)

b: L'ENORME DISGUSTOSO SCHIFOSO VERME verrà recluso per 72 ore in uno di quei ridicoli dispositivi medievali,

b: a meno non sia in realtà *amante* di quel genere di cose,

`bb({body:"scream_a_1"})`

b: dato che è un ENORME DISGUSTOSO SCHIFOSO VERME

`_.a2_attack_3 = "bad";`

`_.a2_hoodie_callback = "the law";`

(#act2d)

# act2c_louder_butterfly

`bb({body:"normal", mouth:"small", eyes:"suspect"})`

b: EFFETTO FARFALLA! Stai usando un bicchiere di plastica non biodegradabile?

`bb({body:"two_up", mouth:"normal", eyes:"shock"})`

b: BAM, UNA DISCARICA RILASCIA VELENO E UCCIDE BAMBINI

`bb({body:"normal", mouth:"small", eyes:"suspect"})`

b: Stai sudando e stai avendo le palpitazioni?

`bb({body:"scream_a_1"})`

b: BAM, SISTEMA SANITARIO IN BANCAROTTA E MILIONI DI VITTIME

`_.a2_attack_3 = "bad";`

`_.a2_hoodie_callback = "the butterfly effect";`

(#act2d)

# act2c_louder_zombies

`bb({body:"normal", mouth:"small", eyes:"angry"})`

b: Questi zombie del piacere ciondoleranno verso di te borbottando:

`bb({body:"normal", mouth:"normal", eyes:"shock"})`

b: MI PIACEEEE. MI PIACEEEEE.

`bb({body:"scream_a_1"})`

b: Poi ti MORDERANNO e ti trasformeranno in un FRA FESSO e/o una CAGNA CRETINA!
`_.a2_attack_3 = "bad";`

`_.a2_hoodie_callback = "zombies";`

(#act2d)

# act2c_louder_hitler

`bb({body:"scream_a_1"})`

b: I NAZI STANNO MARCIANDO PER LE STRADE IN QUESTO MOMENTO

`bb({body:"one_up", mouth:"smile", eyes:"happy"})`

b: Dicendo, *menomale che i "buoni" hanno finito con quelle robe "rilassanti" e "per la cura personale"!*

`bb({body:"point", mouth:"smile", eyes:"happy_r"})`

b: *E ora va tutto SSecondo i piani!*

`_.a2_attack_3 = "bad";`

`_.a2_hoodie_callback = "Hitler";`

(#act2d)

# act2c_louder_ignore

`bb({body:"normal", mouth:"normal", eyes:"normal_r"})`

b: Pensaci, che ne sappiamo se questo posto *non abbia* un rilevatore di monossido?

`bb({body:"two_up", mouth:"small", eyes:"normal"})`

b: E ci stessimo avvelenando *IN QUESTO MOMENTO*?

`bb({body:"scream_a_1"})`

b: NON VEDREMO NEMMENO LA MORTE ARRIVARE. SMETTEREMO SEMPLICEMENTE DI ESISTERE PER SEMPRE E-

`_.a2_attack_3 = "harm";`

`_.a2_hoodie_callback = "carbon monoxide";`

(#act2d)

# act2c_different_social

`bb({body:"normal", mouth:"normal", eyes:"sad"})`

b: E se fossimo *completamente incapaci* di essere amati, o di amare?

`bb({body:"normal", mouth:"small", eyes:"sad_r"})`

b: E se qualcosa dentro di noi si fosse irreversibilmente rotto tempo fa? O non fosse mai del tutto esistito?

`bb({body:"scream_a_1"})`

b: AHH SIAMO COSÌ ROTTI! ROTTI ROTTI ROTTI ROTTI RO-

`_.a2_attack_3 = "alone";`

(#act2d)

# act2c_different_moral

`bb({body:"normal", mouth:"normal", eyes:"normal"})`

b: E se fossimo *completamente marci*?

`bb({body:"one_up", eyes:"sad"})`

b: C'è chi è portato a fare del bene, noi al massimo lo facciamo solo spinti dalla colpa o dalla vergogna.

`bb({body:"normal", mouth:"small", eyes:"sad_r"})`

b: E se fosse nella nostra indole ferire gli altri? E se non fossimo *altro* che un fardello per chi ci sta intorno?

`bb({body:"scream_a_1"})`

b: AHH SIAMO COSÌ ROTTI! ROTTI ROTTI ROTTI ROTTI RO-

`_.a2_attack_3 = "bad";`

(#act2d)

# act2c_punch

`bb({body:"normal", mouth:"normal", eyes:"normal"})`

b: Dico sul serio. Le persone *drogano* le ciotole di punch. È un dato di fatto e succede davvero.

`bb({eyes:"suspect"})`

b: Ti fa male la testa? Ti fanno male gli arti? Mi sa che stiamo morendo.

`bb({body:"scream_a_1"})`

b: AHHH STIAMO MORENDO! STIAMO MORENDO STIAMO MORENDO S-

`_.a2_attack_3 = "harm";`

`_.a2_hoodie_callback = "punch bowls";`

(#act2d)

# act2d

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({body:"attacked"});
attack("20p", _.a2_attack_1);
```

(...401)

```
hong({body:"attacked_2"});
attack("20p", _.a2_attack_2);
```

(...401)

```
hong({body:"attacked_3"});
attack("20p", _.a2_attack_3);
```

(...1001)

h: CAZZOOO!

h: PORCA LA PORCACCIA PORCA MALEDETTAAAAAA

`bb({body:"two_up", mouth:"smile", eyes:"happy"});`

b: Evviva! Son felice mi riesca di nuovo a sentire!

`bb({body:"normal", mouth:"small", eyes:"sad"})`

b: Perché mi stavi ignorando?

`hong({body:"facepalm"})`

h: Porca ^puttana^, brutto imbecille.

`hong({body:"facepalm_2"})`

h: Sai quella storiella nativa americana?

h: "Dentro di noi ci sono due lupi, la speranza e la disperazione, chi dei due vince? Quello che nutri".

```
hong({body:"facepalm_3"});
bb({eyes:"normal"});
```

h: Stavo provando a farti *morire di fame*, brutto ^stronzo^!

`hong({body:"smile", mouth:"smile"})`

h: Al diavolo, dirò delle affermazioni positive.

h: *Sono una persona amata. Gentile, Intelligente. Di bell'aspetto. Speciale*.

`bb({eyes:"suspect"});`

[Accidenti, quanto narcisismo!](#act2d_narcissist)

[Sai che queste affermazioni sono state *smentite?*](#act2d_disproven)

[Ti prego, non associare storielle a caso con gli indigeni](#act2d_racist)

# act2d_disproven

`bb({body:"point", mouth:"normal", eyes:"closed"})`

b: Infatti si possono *ritorcere* contro le persone con un'autostima bassa!

`bb({body:"one_up", mouth:"small", eyes:"normal"})`

b: È stato fatto uno studio randomizzato controllato: chi conduceva la ricerca non sapeva in quale gruppo si trovasse.

`bb({body:"two_up", mouth:"small", eyes:"normal_r"})`

b: Risultato: se hai già un'autostima bassa, ripetere queste affermazioni ti farà sentire *peggio* di non dirle proprio!

`bb({body:"point", mouth:"normal", eyes:"closed"})`

b: Wood 2009, Scienza Psicologica. Controlla su Google Scholar,

`bb({body:"scream_b_1"})`

b: E SMETTILA DI DIFFONDERE BUFALE ANTISCIENTIFICHE

```
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "bad");
```

(...2500)

(#act2e)

# act2d_narcissist

`bb({body:"normal", mouth:"normal", eyes:"normal"})`

b: Se vuoi maturare, *devi* ammettere con umiltà i tuoi difetti!

`bb({body:"two_up", eyes:"suspect"})`

b: Non puoi coprire la polvere con un tappeto! A lungo andare, nascondere i tuoi difetti ti farà stare peggio.

`bb({body:"chest", mouth:"smile", eyes:"closed"})`

b: Per fortuna io, il tuo fedele lupo da guardia, posso avvertirti dei tuoi difetti. E ora va-

`bb({body:"scream_b_1"})`

b: MALE. VA TUTTO MALE

```
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "bad");
```

(...2500)

(#act2e)

# act2d_racist

`bb({body:"normal", mouth:"normal", eyes:"suspect"})`

b: I nativi americani sono *persone*, non "nobili selvaggi" da menzionare per dare un tocco *esotico* alle frasette da Baci Perugina.

`bb({eyes:"suspect_r"})`

b: Stai riducendo degli individui e la loro complessa cultura a una cartolina! È "razzismo a fin di bene"!

`bb({body:"scream_b_1"})`

b: NON ESSERE RAZZISTA, IDIOTA MUSO GIALLO

```
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "bad");
```

(...2500)

(#act2e)

# act2e

h: ^VAFFANCULO^.

`hong({body:"yell", mouth:"yell"})`

h: Sai che c'è? Sei *irrazionale*.

h: Si sa che le emozioni sono irrazionali! Soprattutto la paura!

`hong({body:"facepalm_2"})`

h: Sei un inutile avanzo della crescita, come l'appendice o il dente del giudizio!

`hong({body:"yell", mouth:"yell"})`

h: ^Cazzo^, la metafora del lupo è stupida! Sei solo un mucchio di sostanze neurochimiche del mio cervello.

`hong({body:"cross", mouth:"cross"})`

h: Perché dovrei dar retta a un inesistente, inutile, e irrazionale pezzo di ^merda^ come te?!

`bb({eyes:"sad", MOUTH_LOCK:true})`

b: ...

[Oh, wow. Questo mi ha fatto molto male.](#act2e_hurtful)

[Sono un sentimento. E i sentimenti sono importanti.](#act2e_valid)

[Siamo *entrambi* sostanze chimiche."](#act2e_rational)

# act2e_hurtful

`bb({body:"chest"})`

b: Lo sai, io sono *parte* di te. Quando dici queste cose, fai del male a *te*.

`bb({body:"scream_a_1"})`

b: Quindi, perché ti stai facendo del male? SMETTILA.

```
music(null);
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "harm");
```

(...2500)

(#act2f)

# act2e_rational

`bb({body:"normal", mouth:"normal", eyes:"normal_r"});`

b: Le motivazioni più profonde sono dopamina, le gioie più ricche seratonina.

`bb({body:"one_up"});`

b: I ricordi reti neurali, il buon senso un insieme di segnali elettrici guasti.

`bb({eyes:"normal", body:"normal"});`

b: Se io *sono* irrazionale in quanto "solo sostanza chimica"... allora anche *tu* lo sei!

`bb({body:"two_up", eyes:"shock"});`

b: E se *entrambi* siamo irrazionali, allora non sapremo *mai* come trovare la felicità!
`bb({body:"scream_a_1"})`

b: AHH SIAMO COSÌ ROTTI! ROTTI ROTTI ROTTI ROTTI RO-

```
music(null);
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "bad");
```

(...2500)

(#act2f)

# act2e_valid

`bb({body:"normal", mouth:"normal", eyes:"suspect"});`

b: Un momento... dicono "tutti" che le emozioni sono importanti, che dovresti accettarle.

`bb({eyes:"suspect_r"});`

b: Ma dicono anche che le emozioni sono irrazionali e inaffidabili.

`bb({eyes:"angry"});`

b: Oh no, ci hanno mentito per tutto questo tempo!

`bb({body:"scream_a_1"})`

b: CI HANNO NUTRITO DI CONTRADDIZIONI E RESO SUCCUBI DEL COMPLESSO INDUSTRIALE DI AUTO-AIUTO

```
music(null);
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "harm");
```

(...2500)

(#act2f)

# act2f

`hong({body:"defeated", MOUTH_LOCK:true});`

h: ...

h: Odio tutto questo. Fa così male per quanto lo *odio*.

h: Non riesco a placarti. Ad ignorarti. Ad affrontarti.

`bb({eyes:"suspect"});`

h: Qualunque cosa faccia, non riesco a sbarazzarmi di t-

`bb({body:"cry_1"});`

b: Beh, magari *NON DOVRESTI* SBARAZZARTI DI ME.

`bb({body:"cry_2"});`

b: Come pensi che *io* mi senta?!

`bb({body:"cry_4", mouth:"cry", eyes:"cry"})`

b: Ce la sto mettendo tutta per essere il tuo cane da guardia, ma mi vedi ancora come il lupo cattivo!

b: Sto facendo *del mio meglio* per avvisarti dei pericoli! *Più* pericoli! *Nuovi* pericoli!

`bb({eyes:"cry_2"})`

b: Ma non importa quanto mi sforzi a proteggerti, tu *ancora* pensi che sia il nemico!

`bb({body:"cry_5"});`

b: Dove sto sbagliando?!

`bb({body:"cry_2"});`

b: *So* che faccio schifo nel mio lavoro. Ma ci sto *provando*!

`bb({body:"cry_3"});`

b: Ci sto provando...

`bb({body:"cry_6", mouth:"right", eyes:"cry_r_1"});`

b: Non serve che mi ascolta, che sia d'accordo con me, o che io ti *piaccia*.

`bb({eyes:"cry_r_2"});`

b: Voglio solo che... abbia pazienza con me.

`bb({eyes:"cry_r_3"});`

b: Voglio solo che ti sieda un attimo con me, invece di voltarti e-

```
bb({eyes:"cry_r_4"});
hong({body:"listen"});
```

r: Ehi.

```
hong({body:"look"});
Game.clearText();
publish("act2-in-2");
publish("hp_hide");
music('party1', {volume:0.4, fade:2});
```

(...2000)

```
publish("act2",["party_hunter",2]);
Game.WORDS_HEIGHT_BOTTOM = 230;
```

r: Ehi tu, hai l'aria di aver litigato tra te e te.

```
publish("act2",["party_hunter",3]);
publish("act2",["party_hong",13]);
```

h2: Si vede tanto?

```
publish("act2",["party_hunter",4]);
publish("act2",["party_hong",14]);
```

r: Ehm, stavi bisbigliando con la tua felpa riguardo {{_.a2_hoodie_callback}} o qualcosa del genere.

```
publish("act2",["party_hunter",13]);
publish("act2",["party_hong",15]);
sfx("rustle", {volume:0.6});
setTimeout(function(){
	publish("act2",["party_hong",16]);
	sfx("concrete_step3", {volume:0.6});
},401);
setTimeout(function(){
	publish("act2",["party_hong",17]);
	sfx("concrete_step4", {volume:0.6});
},801);
```

h2: Oddio, sono un disastro.

```
publish("act2",["party_hunter",7]);
publish("act2",["party_hong",18]);
sfx("squeak");
```

r: Ehi. È normalissimo avere l'ansia. Non sei l'unica persona.

```
publish("act2",["party_hunter",5]);
publish("act2",["party_hong",19]);
```

{{if _.act1_ending=="fight"}}
r: Cavolo, proprio ieri al campus ho sentito qualcuno avere un crollo e distruggere il suo telefono!
{{/if}}

{{if _.act1_ending=="flight"}}
r: Cavolo, proprio ieri ho sentito qualcuno rannicchiarsi come un armadillo e piangere in pubblico!
{{/if}}

```
publish("act2",["party_hunter",2]);
```

r: Ascolta: so cosa vuol dire avere quell'animale nella tua testa.

```
publish("act2",["party_hunter",8]);
```

r: *Tutti* lo hanno. Ecco perché faccio feste ogni weekend, per dimenticarci dei problemi e dell'animale.

```
publish("act2",["party_hunter",9]);
publish("act2",["party_hong",20]);
```

h2: Ma la mia ansia...

```
publish("act2",["party_hunter",2]);
publish("act2",["party_hong",21]);
```

r: Non ti preoccupare. Anch'io ero come te, poi ho trovato un trucchetto per far tacere quei pensieri negativi per sempre...

```
publish("act2",["party_hunter",3]);
Game.clearText();
music(null, {fade:1});
```

(...2001)

```
publish("act2",["party_hunter",10]);
publish("act2",["party_hong",22]);
sfx("rustle");
```

(...2501)

```
publish("act2",["party_hunter",10]);
publish("act2",["party_hong",23]);
sfx("rustle2");
```

(...1001)

```
publish("act2",["party_hunter",11]);
```

r: Una mia specialità. Un po' più forte di... beh, in realtà di qualsiasi cosa legale.

```
publish("act2",["party_hunter",12]);
publish("act2",["party_hong",24]);
```

r: Alla salute, ^puttanella^!

```
hong({body:"hold"});
bb({body:"normal", mouth:"small", eyes:"wat"});
Game.clearText();
Game.WORDS_HEIGHT_BOTTOM = -1;
publish("act2-out-3");
publish("hp_show");
```

(...3500)

[Oh mio Dio.](#act2g_1) `Game.OVERRIDE_CHOICE_LINE=true`

[Questo è un pessimo meccanismo di difesa.](#act2g_2) `Game.OVERRIDE_CHOICE_LINE=true`

[Non accettare i drink dagli sconosciuti.](#act2g_3) `Game.OVERRIDE_CHOICE_LINE=true`

# act2g_1

b: O--

(#act2g)

# act2g_2

b: T--

(#act2g)

# act2g_3

b: D--

(#act2g)

# act2g

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("40p", "harm");
```

(...2000)

```
hong({body:"forward", mouth:"forward"});
bb({body:"frazzled", mouth:"frazzled", eyes:"frazzled"});
```

h: Mmh, ha un bel colore!

h: Ha un sapore corposo di "metti a tacere i tuoi pensieri", con un leggero retrogusto di "non sentire più nulla"!

b: Non va bene, umano. Non va per niente bene.

[È *così* che inizia la dipendenza.](#act2h_opt1) `Game.OVERRIDE_CHOICE_LINE=true`

[Lo *sapevo* che stava fuori di festa!](#act2h_opt3) `Game.OVERRIDE_CHOICE_LINE=true`

[Potrebbe aver persino drogato il drink!](#act2h_opt2) `Game.OVERRIDE_CHOICE_LINE=true`


# act2h_opt1

b: È *propr*-

(#act2h)

# act2h_opt2

b: Potrebber aver-

(#act2h)

# act2h_opt3

b: Lo *sapevo* ch-

(#act2h)

# act2h

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("40p", "harm");
```

(...2000)

```
hong({body:"back", mouth:"back"});
bb({body:"panicked", mouth:"panicked", eyes:"panicked"});
```

h: Buonissimo, *e* meno caro di una terapia!

b: PER FAVORE FERMATI

h: Eheheh!

h: E adesso cosa farai *tu*, ^coglione^?

b: Mi dispiace tanto.

b: Mi costringi a usare il mio ATTACCO SPECIALE

```
bb({body:"special_a"});
music('battle', {volume:0.5});
```

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_harm"`

[](#act2h_attack) `_.SPECIAL_ATTACK="harm"; Game.OVERRIDE_CHOICE_LINE=true`

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_alone"`

[](#act2h_attack) `_.SPECIAL_ATTACK="alone"; Game.OVERRIDE_CHOICE_LINE=true`

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_bad"`

[](#act2h_attack) `_.SPECIAL_ATTACK="bad"; Game.OVERRIDE_CHOICE_LINE=true`

# act2h_attack

```
bb({body:"special_b_1"});
hong({body:"forward", mouth:"forward"});
sfx("charging");
```

h: Cos'è questa ^merda^?

h: Dovrai blaterare altre *stupidaggini* con me per-

```
bb({body:"special_c"});
sfx("hadouken");
```

(...901)

(#act2i)

# act2i

```
publish("hide_tabs");
publish("show_special_attack");
Game.FORCE_CANT_SKIP = true;
music(null);
stopAllSounds();
```

(...5000)

```
publish("show_tabs");
hong({ body:"final", mouth:"final" });
bb({ body:"normal", mouth:"normal", eyes:"sad" });
attack("100p", _.SPECIAL_ATTACK);
Game.FORCE_CANT_SKIP = false;
setTimeout(function(){
	publish("remove_special_attack");
},30);
```

(...2500)

h: CHE ^CAZZO^ È STATO?

b: Scusa. Dovevo mostrarti le conseguenze.

{{if _.SPECIAL_ATTACK=="harm"}}
h: POTEVO *VEDERE* IL MIO CADAVERE. HO AVUTO LA *SENSAZIONE* DI MORIRE.
{{/if}}

{{if _.SPECIAL_ATTACK=="alone"}}
h: POTEVO *VEDERE* IL DISPREZZO DI TUTTI. POTEVO *SENTIRE* COSA DICEVANO.
{{/if}}

{{if _.SPECIAL_ATTACK=="bad"}}
h: POTEVO *SENTIRE* LE COSTOLE SCROCCHIARE. POTEVO *SENTIRE* IL SANGUE NELL'ARIA.
{{/if}}

b: Mi dispiace.

n: *DAI IL COLPO DI GRAZIA*

[{LOTTA: Tira fuori i pugni.}](#act2j_fight) `Game.OVERRIDE_CHOICE_LINE=true`

[{FUGA: Andiamocene.}](#act2j_flight) `Game.OVERRIDE_CHOICE_LINE=true`

# act2j_fight

`bb({ eyes:"angry" });`

b: Quella testa bacata si stava approfittando di te.

b: Stava provando a rovinarti, facendoti uscire di testa anche a te!

`bb({ body:"yell_angry_1" });`

b: Prendi a pugni quella ^merda^ e mettila al tappeto!

`bb({ body:"final_1" });`

b:  A PUGNI A PUGNI A PUGNI A PUGNI A PUGNI A PUGNI A PUGNI A PUGNI A PUGNI A PUGNI A-

`_.a2_ending = "fight";`

(#act2k)

# act2j_flight

b: Lo *sapevo* che questi festaioli erano tutti matti. Alleviano il dolore con delle cose orribili!

`bb({ body:"yell_1" });`

b: E ti sta incastrando a fare lo stesso! Ti sta rovinando! Dobbiamo andarcene via!

`bb({ body:"final_1" });`

b: VAI VIA VAI VIA VAI VIA VAI VIA VAI VIA VAI VIA VAI VIA VAI VIA VAI VIA VAI VIA-

`_.a2_ending = "flight";`

(#act2k)

# act2k

```
Game.clearText();
publish("act2-in-4");
publish("hp_hide");
music('party1', {volume:0.6, fade:1.5});
```

(...2001)

```
publish("act2",["party_hong",26]);
sfx("slide");
```

(...1001)

```
publish("act2",["party_hunter",14]);
Game.WORDS_HEIGHT_BOTTOM = 230;
```

r: Va tutto bene?

`publish("act2",["party_hunter",13]);`

{{if _.a2_ending=="fight"}}
(#act2k_fight)
{{/if}}

{{if _.a2_ending=="flight"}}
(#act2k_flight)
{{/if}}

# act2k_fight

```
Game.clearText();
publish("act2",["party_hunter",21]);
publish("act2",["party_hong",33]);
music(null);
sfx("hit");
```

(...1000)

```
sfx("record_scratch");
publish("act2",["party_hunter",22]);
publish("act2",["party_hong",34]);
publish("act2",["dee",6]);
publish("act2",["dum",6]);
```

r: T-tu...

```
publish("act2",["party_hunter",23]);
publish("act2",["party_hong",35]);
publish("act2",["dee",5]);
publish("act2",["dum",5]);
music('party1', {volume:0.6, fade:6});
```

r: stai *fuori*.

r: Forte. Ti aspetto per il prossimo weekend, tesoro.

```
publish("act2",["party_hunter",19]);
publish("act2",["party_hong",36]);
```

h2: Ok ciao, bye, adiós, au revoir

r: L'animale potrebbe aver vinto oggi, ma tu torna, e ti preparerò qualcosa di ancora più forte!

h2: Sayōnara, auf wiedersehen, zài jiàn, shalom

r: Faremo vedere a quella bestia chi è che comanda!

(#act2k_end)

# act2k_flight

`publish("act2",["party_hong",36]);`

h2: Ok scusa devo scappare.

`publish("act2",["party_hunter",16]);`

r: Cavolo. Oggi ha vinto l'animale, eh?

`publish("act2",["party_hunter",15]);`

h2: No no, devo, ehm, fare una maratona. Devo andare veloce!

`publish("act2",["party_hunter",19]);`

r: Torna il prossimo weekend, tesoro. Ti preparerò qualcosa di ancora più forte.

h2: Ok grazie ora devo proprio correre!

r: Faremo vedere a quella bestia chi è che comanda!

(#act2k_end)

# act2k_end

```
Game.clearText();
publish("act2-out-5");
publish("act2-outro", ["end1"]);
music("hum", {fade:2, volume:0.6});
Game.WORDS_HEIGHT_BOTTOM = -1;
```

(...2500)

```
publish("act2", ["act2_end",2]);
sfx("whoosh");
```

(...1000)

b: Umano! Tutto bene?!

```
publish("act2", ["act2_end","next"]);
```

b: Cavolo, c'è mancato *poco*. Potevamo-

```
Game.clearText();
publish("act2", ["act2_end","next"]);
music(null);
sfx("squeak");
```

(...1500)

```
publish("act2", ["act2_end","next"]);
sfx("hit");
```

(...1000)

h: Tornerò alla festa il prossimo weekend.

h: La prossima volta, non ti *metterò al tappeto* e basta...

h: Ti *ucciderò*, ^cazzo^.

```
Game.clearText();
publish("act2", ["act2_end","next"]);
sfx("concrete_step1");
````

(...901)

```
publish("act2", ["act2_end","next"]);
sfx("concrete_step2", {volume:0.8});
```

(...901)

```
publish("act2", ["act2_end","next"]);
sfx("concrete_step3", {volume:0.5});
```

(...901)

`sfx("concrete_step4", {volume:0.25});`

(...3000)

`_.INTERMISSION_STAGE = 2;`

(#intermission)
