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

s: Ma hai visto la "storia-notizia" su quell'orribile cosa successa non so dove?But did you *see* that "news story" about that horrible thing happening somewhere?

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

a: Dio, odio quegli articoli. Tutto sensazionalismo per farti cliccare.God I hate the news. It's all sensationalism and clickbait.

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

s: Hai ragione, ma lo fanno solo per incentivare. Il *vero* problema è chi ci clicca.True, but they're just following incentives. The *real* problem is people who click the clickbait.

```
publish("act2",["dee",3]);
```

s: Chi retwitterebbe mai una storia così terribile e far star male i suoi amici?Who would retweet a terrible news story, and make all their friends feel bad?

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

s: Ma hai *visto* quella "storia notizia" andata virale?

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

a: Già, palesemente una bufala. Chi ci crederebbe mai e la retwitterebbe?

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

s: Sul serio, amico. Cioè, tutto bene? Ma andare su Google e verificare prima?

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

h2: n... nice party...

```
publish("act2",["party_hong","next"]);
publish("act2",["party_hunter",0]);
publish("act2",["dee",1]);
```

s: Beh, ieri ho visto qualcuno retwittare una GIF di un gatto che beve il latte.

```
publish("act2",["dee",3]);
```

s: Ma non lo possono digerire! Chi mai retwitterebbe un *abuso sugli animali* del genere?

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

s: Ma che ne so! Cos'è, pensa forse che sia *serial killer* o qualcosa del genere? Quanta paranoia.

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

s: Ma che ne so! Pensa forse che gli incontri non possano colmare il vuoto nel suo cuore?

s: Quanto sei moralista! Apri la mente, poi le gambe!

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

b: Stiamo rovinando l'atmosfera della festa facendo i musoni!

`bb({eyes:"shock", body:"two_up"})`

b: Stiamo uccidendo l'atmosfera! Stiamo commettendo un atmosfericidio di primo grado!

`bb({eyes:"normal", body:"normal"})`

b: Umano, dobbiamo andarcene *ora*, prima che-

```
_.a2_first_danger = 'social';
_.a2_attack_1 = "alone";
```

(#act2b)

# act2a_perv

`bb({eyes:"suspect"})`

b: È più attraente di noi, vuol dire che ci mettiamo a *fissare*, allora-

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

b: Contribuire all'umanità? Tutti i grandi lavori deteriorano la via di Osimandia. Amare? Alla fine moriremo tutti.All great works decay the way of Ozymandias. Love? Death will always do it part.

`bb({eyes:"sad_r"})`

b: E quanta morte c'è! *Noi* moriremo. *I nostri cari* moriranno.

`bb({eyes:"shock", body:"two_up"})`

b: Cavolo, la Seconda Legge della Termodinamica Heck dimostra che anche il nostro *universo* morirà!

`bb({eyes:"suspect", body:"normal"})`

b: Oh, "la morte ci fa apprezzare la vita"? È come dire che la schiavitù è bella perché ci fa apprezzare la libertà!

`bb({body:"one_up"})`

b: Oh, "dai un senso alla tua esistenza"? È quello che fanno i cultisti e i cospirazionisti!

`bb({eyes:"shock", body:"two_up"})`

b: La vita non ha senso, la morte non ha senso, neanche il *senso* ha senso! Un'anima mortale che dovrebbe-

```
_.a2_first_danger = 'meaning';
_.a2_attack_1 = "bad";
```

(#act2b)

# act2b

`bb({eyes:"normal", mouth:"normal", body:"normal", MOUTH_LOCK:true})`

b: ...

`bb({eyes:"suspect"})`

b: Ehm... mi senti, umano?

`bb({eyes:"normal", MOUTH_LOCK:true})`

b: ...

`bb({eyes:"shock", mouth:"small_talk", body:"chest", MOUTH_LOCK:true})`

b: *AHHH*

`bb({mouth:"small_talk"})`

b: TI DEVO AVVISARE DI...

[*Altri pericoli* dello stesso pericolo!](#act2b_louder)

{{if _.a2_first_danger=="social"}}
[Un *nuovo* pericolo sociale!](#act2b_different_social)
{{/if}}

{{if _.a2_first_danger=="perv" || _.a2_first_danger=="meaning"}}
[Un *nuovo* pericolo morale!](#act2b_different_moral)
{{/if}}

[Stai ignorando il pericolo! È pericoloso!](#act2b_ignore)

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

b: "UN ENORME, DISGUSTOSO, SCHIFOSO PERVERTITO"

```
_.a2_second_danger = 'law';
_.a2_attack_2 = "bad";
_.a2_hoodie_callback = "the law";
```

(#act2c)

# act2b_louder_meaning

`bb({body:"two_up", mouth:"normal", eyes:"shock"})`

b: In realtà, anche se trovassi un valido scopo nella vita, puoi *sempre* rovinare tutto!

`bb({body:"normal", mouth:"normal", eyes:"normal"})`

b: Alfred Nobel voleva la pace nel mondo e che le culture socializzassero Quindi, ha deciso di semplificare i viaggi.

`bb({eyes:"normal_r"})`

b: Gli serviva un modo economico per creare dei tunnel per i treni. E così, inventò un materiale chiamato "dinamite"...

`bb({body:"one_up", eyes:"normal"})`

b: Utilizzata nella I Guerra Mondiale per UCCIDERE MILIONI DI PERSONE

`bb({body:"two_up", eyes:"shock"})`

b: È L'EFFETTO FARFALLA, UMANO! STAI UCCIDENDO UN SACCO DI PERSONE IN QUESTO MOMENTO

```
_.a2_second_danger = 'butterfly';
_.a2_attack_2 = "bad";
_.a2_hoodie_callback = "World War I";
```

(#act2c)

# act2b_different_social

`_.a2_first_choice = "different"`

`bb({eyes:"normal_r", body:"point", mouth:"normal"})`

b: A dire il vero, sai cosa c'è di peggio di non essere amati da nessuno? Essere amati da *tutti*.

`bb({body:"one_up", eyes:"suspect", mouth:"normal"})`

b: E diventare come *questi* animali da festa a caccia di piaceri.

`bb({body:"normal", mouth:"small"})`

b: Una vita superificiale con amici superficiali possono solo conoscere la parte superficiale di te!

`bb({body:"two_up", eyes:"shock", mouth:"normal"})`

b: Umano, dobbiamo scappare da questi zombie del piacere, prima che ci fanno diventare come loro!

```
_.a2_second_danger = 'zombies';
_.a2_attack_2 = "alone";
_.a2_hoodie_callback = "zombies";
```

(#act2c)

# act2b_different_moral

`_.a2_first_choice = "different"`

`bb({body:"two_up", eyes:"shock", mouth:"normal"})`

b: *In questo momento*c'è chi muore nelle carestie e nei genodici, e noi stiamo facendo festa!

`bb({body:"point", eyes:"closed", mouth:"small"})`

b: Un saggio disse, "l'unica cosa necessaria per far sì che il male trionfi è che i buoni non facciano nulla."

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

b: Pensi di essere al sicuro solo perché hai tolto le batterie dal rilevatore di monossido di carbonio?

`bb({eyes:"suspect_r"})`

b: Non riuscirai nemmeno a sentirne l'odore! Ti addormenterai e poi-

`bb({body:"scream_c_1"})`

b: MORIRAIIIIIIIIII

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

b: Oh, menomale, umano, mi sa che ora mi senti!

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

b: Actually, Netflix & food delivery isn't quarantined enough! We'd still infect the delivery person!

`bb({body:"one_up", mouth:"small"})`

b: We need to move to the Canadian Yukon territories, and have our food delivered by drone!

`bb({body:"two_up", mouth:"normal"})`

b: And then they'd have to sterilize the drone to rid it of our SAD LUMP GERMS

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

b: The BIG DISGUSTING TRASH PERVERT shall be sentenced to 72 hours in one of those medieval public-humiliation devices

b: unless they're secretly *into* that sort of thing

`bb({body:"scream_a_1"})`

b: because they're a BIG DISGUSTING TRASH PERVERT

`_.a2_attack_3 = "bad";`

`_.a2_hoodie_callback = "the law";`

(#act2d)

# act2c_louder_butterfly

`bb({body:"normal", mouth:"small", eyes:"suspect"})`

b: BUTTERFLY EFFECT! You're using a non-biodegradable plastic cup?

`bb({body:"two_up", mouth:"normal", eyes:"shock"})`

b: BAM, A LANDFILL LEAKS POISON AND KILLS A KID

`bb({body:"normal", mouth:"small", eyes:"suspect"})`

b: You're sweating and your heart's pounding?

`bb({body:"scream_a_1"})`

b: BAM, YOU BANKRUPT OUR HEALTHCARE SYSTEM AND MILLIONS DIE

`_.a2_attack_3 = "bad";`

`_.a2_hoodie_callback = "the butterfly effect";`

(#act2d)

# act2c_louder_zombies

`bb({body:"normal", mouth:"small", eyes:"angry"})`

b: These pleasure-zombies will stumble towards you mumbling,

`bb({body:"normal", mouth:"normal", eyes:"shock"})`

b: LIIIIIKES. LIIIIIIIIIIKES.

`bb({body:"scream_a_1"})`

b: Then they'll BITE YOU and turn you into a BRAINLESS BRO and/or THOUGHTLESS THOT!

`_.a2_attack_3 = "bad";`

`_.a2_hoodie_callback = "zombies";`

(#act2d)

# act2c_louder_hitler

`bb({body:"scream_a_1"})`

b: THE NAZIS ARE GOOSE-STEPPING BACK ON THE STREETS RIGHT NOW

`bb({body:"one_up", mouth:"smile", eyes:"happy"})`

b: Saying, *good thing those 'good folks' slacked off with stuff like 'relaxing' and 'self-care'!*

`bb({body:"point", mouth:"smile", eyes:"happy_r"})`

b: *Now our plans can go fourth, reich on schedule!*

`_.a2_attack_3 = "bad";`

`_.a2_hoodie_callback = "Hitler";`

(#act2d)

# act2c_louder_ignore

`bb({body:"normal", mouth:"normal", eyes:"normal_r"})`

b: Come to think about it, do we know if this building *has* a monoxide detector?!

`bb({body:"two_up", mouth:"small", eyes:"normal"})`

b: What if we're all being poisoned *RIGHT NOW?*

`bb({body:"scream_a_1"})`

b: WE WOULDN'T EVEN SEE DEATH APPROACH. WE'D JUST STOP EXISTING FOREVER AND EVER AND EV--

`_.a2_attack_3 = "harm";`

`_.a2_hoodie_callback = "carbon monoxide";`

(#act2d)

# act2c_different_social

`bb({body:"normal", mouth:"normal", eyes:"sad"})`

b: What if we're just *fundamentally incapable* of ever being loved, or loving another?

`bb({body:"normal", mouth:"small", eyes:"sad_r"})`

b: What if something irreversibly broke inside of us a long time ago? Or never existed in us in the first place?

`bb({body:"scream_a_1"})`

b: AHH WE'RE BROKEN! SO BROKEN SO BROKEN SO BROKE--

`_.a2_attack_3 = "alone";`

(#act2d)

# act2c_different_moral

`bb({body:"normal", mouth:"normal", eyes:"normal"})`

b: What if we're just *fundamentally rotten?*

`bb({body:"one_up", eyes:"sad"})`

b: Others have an inner drive to do goodness, but we only do "good" out of guilt or shame, if at all.

`bb({body:"normal", mouth:"small", eyes:"sad_r"})`

b: What if it's in our nature to hurt others? What if we can't be anything *other* than a burden to those close to us?

`bb({body:"scream_a_1"})`

b: AHH WE'RE BROKEN! SO BROKEN SO BROKEN SO BROKE--

`_.a2_attack_3 = "bad";`

(#act2d)

# act2c_punch

`bb({body:"normal", mouth:"normal", eyes:"normal"})`

b: I'm not being irrational. People *do* drug punch bowls. That is an actual thing that actually happens.

`bb({eyes:"suspect"})`

b: Human, does your head hurt? Are your limbs limp? I think we're dying.

`bb({body:"scream_a_1"})`

b: AHHH WE'RE DYING! WE'RE DYING WE'RE DYING WE'RE DYI--

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

h: F^AAACK^!

h: F^ACK^ING F^ACK^-F^AKK^ITY *F^AAAAACK^*

`bb({body:"two_up", mouth:"smile", eyes:"happy"});`

b: Yay, human! I'm so happy you can hear me again!

`bb({body:"normal", mouth:"small", eyes:"sad"})`

b: Why were you ignoring me?

`hong({body:"facepalm"})`

h: Holy ^hell^, you absolute moron.

`hong({body:"facepalm_2"})`

h: You know that Native American story?

h: "There are two wolves inside you, one is hope, one is despair, which wolf wins? The one you feed."

```
hong({body:"facepalm_3"});
bb({eyes:"normal"});
```

h: I was trying to *starve* you, you sadistic ^asshole^!

`hong({body:"smile", mouth:"smile"})`

h: Screw it, I'll do positive affirmations instead.

h: *I am loved. I am good. I am smart. I am beautiful. I am special.*

`bb({eyes:"suspect"});`

[Golly, that's so narcissistic!](#act2d_narcissist)

[Y'know affirmations were *disproven?*](#act2d_disproven)

[omg don't credit random stories to indigenous folk](#act2d_racist)

# act2d_disproven

`bb({body:"point", mouth:"normal", eyes:"closed"})`

b: In fact, they actually *backfire* for people with low self-esteem! 

`bb({body:"one_up", mouth:"small", eyes:"normal"})`

b: It was a well-designed study – randomized controlled trial, experimenter was blinded as to who was in which group.

`bb({body:"two_up", mouth:"small", eyes:"normal_r"})`

b: Results: if you already had low self-esteem, being asked to repeat affirmations makes you feel *worse* than if you'd said nothing at all!

`bb({body:"point", mouth:"normal", eyes:"closed"})`

b: Wood 2009, Psychological Science. Look it up on Google Scholar, human,

`bb({body:"scream_b_1"})`

b: THEN STOP SPREADING UNSCIENTIFIC FAKE NEWS

```
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "bad");
```

(...2500)

(#act2e)

# act2d_narcissist

`bb({body:"normal", mouth:"normal", eyes:"normal"})`

b: You *need* to humbly see your own flaws in order to grow as a person!

`bb({body:"two_up", eyes:"suspect"})`

b: You can't spray air freshener over a moldy room! Covering up your flaws makes you worse in the long run.

`bb({body:"chest", mouth:"smile", eyes:"closed"})`

b: Thankfully, I, as your loyal guard-wolf, can alert you to your flaws. And right now, it's-

`bb({body:"scream_b_1"})`

b: EVERYTHING. EVERYTHING IS WRONG

```
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "bad");
```

(...2500)

(#act2e)

# act2d_racist

`bb({body:"normal", mouth:"normal", eyes:"suspect"})`

b: Native Americans are *actual people*, not some "noble savages" you can namedrop to make your fortune-cookie advice more *exotic*.

`bb({eyes:"suspect_r"})`

b: You're reducing individual persons & complex cultures to a Hallmark card! That's "benevolent racism"! 

`bb({body:"scream_b_1"})`

b: STOP BEING RACIST YOU SQUINTY-EYED JERK

```
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "bad");
```

(...2500)

(#act2e)

# act2e

h: ^ASSDAMMIT^.

`hong({body:"yell", mouth:"yell"})`

h: You know what? You're *irrational*.

h: Everyone knows emotions are irrational! Especially fear!

`hong({body:"facepalm_2"})`

h: You're a useless evolutionary leftover, like my appendix or wisdom teeth!

`hong({body:"yell", mouth:"yell"})`

h: ^Hell^, this whole wolf metaphor is stupid! You're just a bunch of neuro-chemicals in my head.

`hong({body:"cross", mouth:"cross"})`

h: So why should I listen to a worthless, irrational, non-existent piece of ^shit^ like you?!

`bb({eyes:"sad", MOUTH_LOCK:true})`

b: ...

[Jeez, human. That's really hurtful.](#act2e_hurtful)

[I'm a feeling. Feelings are valid.](#act2e_valid)

[Human, we're *both* "just chemicals."](#act2e_rational)

# act2e_hurtful

`bb({body:"chest"})`

b: I'm *part* of you, you know. When you say that, you're hurting *yourself*.

`bb({body:"scream_a_1"})`

b: Why are you hitting yourself, human? STOP HITTING YOURSELF.

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

b: Your deepest motivations are dopamine, your richest joys are serotonin.

`bb({body:"one_up"});`

b: Your memories are synaptic weights, your reason is fault-prone electrical signals.

`bb({eyes:"normal", body:"normal"});`

b: So if me being "just chemicals" means *I'm* irrational... then that means *you're* irrational!

`bb({body:"two_up", eyes:"shock"});`

b: And if we're *both* irrational, then we'll *never* figure out how to be fulfilled and happy!

`bb({body:"scream_a_1"})`

b: AHHH WE'RE BROKEN! SO BROKEN SO BROKEN SO BROKEN--

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

b: Hang on... "they" say that feelings are valid, that you should always accept your emotions.

`bb({eyes:"suspect_r"});`

b: But "they" also say emotions are irrational, that emotions are not to be trusted.

`bb({eyes:"angry"});`

b: Oh my gosh, "they" have been lying to us this whole time!

`bb({body:"scream_a_1"})`

b: "THEY" FEED US CONTRADICTIONS TO MAKE US DEPENDENT ON THE SELF-HELP INDUSTRIAL COMPLEX

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

h: I hate this. God it hurts so much I *hate* this.

h: I can't appease you. I can't ignore you. I can't fight you. 

`bb({eyes:"suspect"});`

h: No matter what I do, I can't seem to get rid of yo--

`bb({body:"cry_1"});`

b: Well maybe you're NOT *SUPPOSED* TO GET RID OF ME.

`bb({body:"cry_2"});`

b: How do you think *I* feel, human?!

`bb({body:"cry_4", mouth:"cry", eyes:"cry"})`

b: I'm trying my best to be your guard-dog, but you keep seeing me as some Big Bad Wolf!

b: So I try even *harder* to alert you to danger! *More* danger! *Different* danger!

`bb({eyes:"cry_2"})`

b: But no matter how hard I try to protect you, you *still* think I'm your enemy!

`bb({body:"cry_5"});`

b: What am I doing wrong?!

`bb({body:"cry_2"});`

b: I *know* I suck at my job. But I'm *trying*, human!

`bb({body:"cry_3"});`

b: ...I'm trying.

`bb({body:"cry_6", mouth:"right", eyes:"cry_r_1"});`

b: You don't have to heed my warnings, or agree with me, or even *like* me.

`bb({eyes:"cry_r_2"});`

b: I just... all I want is for you to be patient with me.

`bb({eyes:"cry_r_3"});`

b: I just want for you to sit with me for a while, instead of turning away and--

```
bb({eyes:"cry_r_4"});
hong({body:"listen"});
```

r: Hey.

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

r: Looks like you're caught in a fight with yourself, kid.

```
publish("act2",["party_hunter",3]);
publish("act2",["party_hong",13]);
```

h2: Was it that obvious?

```
publish("act2",["party_hunter",4]);
publish("act2",["party_hong",14]);
```

r: You were, uh, mumbling at your hoodie about {{_.a2_hoodie_callback}} or something.

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

h2: oh god i'm such a mess.

```
publish("act2",["party_hunter",7]);
publish("act2",["party_hong",18]);
sfx("squeak");
```

r: Hey. You're not alone, friend. Anxiety's super common.

```
publish("act2",["party_hunter",5]);
publish("act2",["party_hong",19]);
```

{{if _.act1_ending=="fight"}}
r: Heck, just yesterday, I heard someone on campus had a nervous breakdown and smashed their phone!
{{/if}}

{{if _.act1_ending=="flight"}}
r: Heck, just yesterday, I heard someone curled up into an armadillo ball and cried in public!
{{/if}}

```
publish("act2",["party_hunter",2]);
```

r: Listen: I know what it's like to have that animal in your head.

```
publish("act2",["party_hunter",8]);
```

r: We *all* do. That's why I throw these parties every weekend, to forget our worries, forget that animal.

```
publish("act2",["party_hunter",9]);
publish("act2",["party_hong",20]);
```

h2: but my anxiety...

```
publish("act2",["party_hunter",2]);
publish("act2",["party_hong",21]);
```

r: Don't worry, kid. I used to be like you. But then I found a little trick to get that negative voice to shut up forever...

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

r: My own specialty blend. It's a bit stronger than... well, anything legal really.

```
publish("act2",["party_hunter",12]);
publish("act2",["party_hong",24]);
```

r: Bottoms up, ^bee-yatch^!

```
hong({body:"hold"});
bb({body:"normal", mouth:"small", eyes:"wat"});
Game.clearText();
Game.WORDS_HEIGHT_BOTTOM = -1;
publish("act2-out-3");
publish("hp_show");
```

(...3500)

[Oh my God.](#act2g_1) `Game.OVERRIDE_CHOICE_LINE=true`

[This is a bad coping mechanism.](#act2g_2) `Game.OVERRIDE_CHOICE_LINE=true`

[Don't take drinks from strangers.](#act2g_3) `Game.OVERRIDE_CHOICE_LINE=true`

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

h: Mmm, what an exquisite palette!

h: A full-bodied flavor of "shut your mind up," with a subtle aftertaste of "never feel anything ever again"!

b: This is bad, human. This is really, really bad.

[This is *actually* how addiction starts.](#act2h_opt1) `Game.OVERRIDE_CHOICE_LINE=true`

[I *knew* the host was deeply messed up!](#act2h_opt3) `Game.OVERRIDE_CHOICE_LINE=true`

[Also, they could have drugged that!](#act2h_opt2) `Game.OVERRIDE_CHOICE_LINE=true`


# act2h_opt1

b: This is *actu*--

(#act2h)

# act2h_opt2

b: Also, they co--

(#act2h)

# act2h_opt3

b: I *knew* th--

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

h: Delicious, *and* cheaper than therapy!

b: HUMAN PLEASE STOP

h: Hehehe!

h: And what are *you* gonna do about it, ^asshole^?

b: I'm so sorry, human.

b: I'm going to have to use my SPECIAL ATTACK

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

h: What's this ^crap^?

h: You're gonna yap more stupid *words* at me to--

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

h: WHAT THE ^HELL^ WAS THAT

b: I'm sorry. I needed to show you the consequences.

{{if _.SPECIAL_ATTACK=="harm"}}
h: I COULD *SEE* MY OWN CORPSE. I COULD *FEEL* THE SENSATION OF BEING ACTUALLY DEAD.
{{/if}}

{{if _.SPECIAL_ATTACK=="alone"}}
h: I COULD *SEE* EVERYONE'S LOOK OF DISGUST. I COULD *HEAR* ALL THE THINGS THEY SAID.
{{/if}}

{{if _.SPECIAL_ATTACK=="bad"}}
h: I COULD *HEAR* THE CRUNCHING OF RIBS. I COULD *TASTE* THE BLOOD IN THE AIR.
{{/if}}

b: I'm sorry, human.

n: *FINISH THEM*

[{FIGHT: Punch the host.}](#act2j_fight) `Game.OVERRIDE_CHOICE_LINE=true`

[{FLIGHT: Let's get out of here.}](#act2j_flight) `Game.OVERRIDE_CHOICE_LINE=true`

# act2j_fight

`bb({ eyes:"angry" });`

b: That psychopath was taking advantage of you.

b: They were trying to corrupt you, make you as messed up as they are!

`bb({ body:"yell_angry_1" });`

b: Punch that jerk! Knock their friggin' lights out!

`bb({ body:"final_1" });`

b: PUNCH THEM PUNCH THEM PUNCH THEM PUNCH THEM PUNCH THEM PUNCH THEM PUNCH THEM PUNCH THE--

`_.a2_ending = "fight";`

(#act2k)

# act2j_flight

b: I *knew* all these partygoers were deeply messed up. They all dull their pain with horrible things!

`bb({ body:"yell_1" });`

b: And they're tricking you into doing the same thing! They're corrupting you! We need to get out!

`bb({ body:"final_1" });`

b: GET OUT GET OUT GET OUT GET OUT GET OUT GET OUT GET OUT GET OUT GET OUT GET OU--

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

r: You alright, kid?

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

r: Y-you...

```
publish("act2",["party_hunter",23]);
publish("act2",["party_hong",35]);
publish("act2",["dee",5]);
publish("act2",["dum",5]);
music('party1', {volume:0.6, fade:6});
```

r: are *kinky*.

r: I like that. Come to my party next weekend, cutie.

```
publish("act2",["party_hunter",19]);
publish("act2",["party_hong",36]);
```

h2: ok bye, ciao, adios, au revoir

r: The animal might have won today, but come back, and I'll mix something even stronger for you!

h2: sayōnara, auf wiedersehen, zài jiàn, shalom

r: You and me, kid, we'll show that beast who's boss!

(#act2k_end)

# act2k_flight

`publish("act2",["party_hong",36]);`

h2: ok sorry i have to run

`publish("act2",["party_hunter",16]);`

r: ^Damn^ it. The animal won today, huh?

`publish("act2",["party_hunter",15]);`

h2: no no, just, uh, gotta run a marathon. gotta go fast.

`publish("act2",["party_hunter",19]);`

r: Come to my party next weekend, cutie. I'll mix something even stronger for you.

h2: ok thanks gonna run run run run run

r: You and me, kid, we'll show that beast who's boss!

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

b: Human! Are you okay?!

```
publish("act2", ["act2_end","next"]);
```

b: Gosh, that was *close.* We really could've--

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

h: I'm coming back to the party next weekend.

h: The next time we fight, I'm not just going to *defeat* you...

h: I'm going to ^fuck^ing *kill* you.

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
