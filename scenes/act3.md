# act3

```
SceneSetup.act3();
Game.WORDS_HEIGHT_BOTTOM = 205;
sfx("cheers");
```

r: Cheers!

```
publish("act3",["roofhunter",1]);
publish("act3",["roofhong",1]);
sfx("drinking");
```

(...4001)

```
publish("act3-alpha", ["dizzyhunter",1]);
publish("act3-alpha", ["dizzyhong",1]);
publish("act3",["roofhunter",3]);
publish("act3",["roofhong",3]);
```

h2: *Ah* that hits the spot.

```
publish("act3",["roofhunter",2]);
publish("act3",["roofhong",2]);
```

r: You know, kid...

```
publish("act3",["roofhunter",3]);
publish("act3",["roofhong",6]);
```

h2: Specifically, the spots hit are my left and right amygdala.

```
publish("act3",["roofhunter",8]);
publish("act3",["roofhong",5]);
```

r: Mi ricordi quando avevo la tua età. Quando l'animale nella mia testa mi tormentava.

```
publish("act3",["roofhunter",9]);
publish("act3",["roofhong",2]);
```

r: I'm so grateful I can pay it forward, and help you kill the beast the way I killed mine.

```
publish("act3",["roofhunter",2]);
```

r: Ehi, domanda al volo: obbligo o ve-

```
publish("act3",["roofhunter",3]);
publish("act3",["roofhong",7]);
publish("act3-alpha", ["dizzyhong",0]);
```

h2: OBBLIGO!

```
publish("act3-alpha", ["dizzyhong",1]);
publish("act3",["roofhunter",10]);
publish("act3",["roofhong",2]);
```

r: Ahah! Bene.

```
publish("act3",["roofhunter",21]);
publish("act3",["roofhong",4]);
```

r: Ok. Vedi quella piscina azzurra laggiù?

```
publish("act3-alpha", ["dizzyhong",0]);
publish("act3",["roofhunter",11]);
publish("act3",["roofhong",9]);
```

h2: Yeah? Six floors down?

```
publish("act3",["roofhunter",10]);
publish("act3",["roofhong",8]);
```

r: Tuffatici.

```
publish("act3",["roofhunter",11]);
publish("act3",["roofhong",10]);
```

h2: ...

```
publish("act3",["roofhong",11]);
```

h2: Aspetta, cosa?

```
publish("act3",["roofhong",10]);
publish("act3",["roofhunter",2]);
```

r: The animal's started whining, hasn't it?

```
publish("act3",["roofhunter",23]);
```

r: *Oh nooooo è pericolo, non farlooooo*

```
publish("act3",["roofhunter",22]);
```

r: But that's exactly why we need death-defying thrills! Party hard! Carpe diem! Snort coke off a hooker's ^ass^, #YOLO!

```
publish("act3",["roofhunter",10]);
```

r: Fai vedere all'animale che non ce ne frega un *^cazzo^* delle sue ^stronzate^! Salta.

```
publish("act3",["roofhunter",11]);
publish("act3",["roofhong",13]);
```

h2: Oh, ma a volte, ehm... è giusto aver paura...

```
publish("act3",["roofhunter",5]);
publish("act3",["roofhong",12]);
music(null, {fade:2});
```

r: ...

```
publish("act3-alpha", ["dizzyhunter",0]);
publish("act3",["roofhunter",6]);
publish("act3",["dd",1]);
```

r: Scusa, did you fall for that McMindfulness propaganda that claims feeling bad is *good?*

```
publish("act3",["roofhunter",17]);
```

r: The ^assholes^ who run this world give the rest of *us* anxiety and depression,

```
publish("act3",["roofhunter",18]);
```

r: Then make TED Talks to tell us to "accept" being ^fucked^ over, and "embrace" that sadistic demon in our heads!

```
publish("act3",["roofhunter",6]);
```

r: Kid, I know that *you* know that animal *hurts* people like us. It *tortures* people like us.

```
publish("act3",["roofhunter",19]);
```

r: Non è un amico. It's a rabid beast, which either needs to be *tranquilized*,

```
publish("act3",["roofhunter",20]);
```

r: Or have a *bullet put in its skull*.

```
publish("act3",["roofhunter",27]);
```

r: Altrimenti lo lascerai vincere.

```
publish("act3",["roofhunter",31]);
publish("act3",["roofhong",14]);
publish("act3",["dd",2]);
```

h2: No. Ti sbagli.

```
publish("act3",["roofhunter",13]);
publish("act3",["roofhong",15]);
music('battle_dark', {volume:1.0}, function(){
	music('battle_dark_loop');
});
```

h2: Non lo lascerò vincere.

```
publish("act3",["roofhunter",25]);
publish("act3-alpha", ["roofhong",0]);
publish("act3-alpha", ["transition",1]);
publish("act3",["dd",6]);
```

r: Sì, ^cazzo^! Io credo in te, tesoro! Uccidilo! <3

(#act3a)



# act3a

```
Game.clearText();
publish("act3-out");
Game.WORDS_HEIGHT_BOTTOM = -1; /* reset */
_.act3_bb_body = 1;
```

(...1500)

```
publish("hp_show");
```

b: no no no no no no

n: QUESTO CAPITOLO HA DUE POSSIBILI FINALI. ONE IS *VERY, VERY BAD.*

b: NO NO NO NO NO NO NO NO NO NO NO NO NO NO

n: SCEGLI ATTENTAMENTE. PROTEGGI IL TUO UMANO

`bb({ eyes:"oh_crap", mouth:"normal_talk", MOUTH_LOCK:true });`

b: AAAAAAAAAAAAAAAAAA

`bb({ mouth:"normal" });`

n: IN BOCCA AL LUPO

```
Game.clearText();
bb({ eyes:"start" });
```

[Umano, qui potresti veramente MORIRE!](#act3a_harm) `Game.OVERRIDE_CHOICE_LINE=true`

[Questo è stupido ed autodistruttivo!](#act3a_bad) `Game.OVERRIDE_CHOICE_LINE=true`

[Questi pazzi non sono tuoi amici!](#act3a_alone) `Game.OVERRIDE_CHOICE_LINE=true`

# act3a_harm

`bb({ MOUTH_LOCK:true, mouth:"normal_talk" });`

b: U-

(#act3a_after)

# act3a_alone

`bb({ MOUTH_LOCK:true, mouth:"normal_talk" });`

b: Q--

(#act3a_after)

# act3a_bad

`bb({ MOUTH_LOCK:true, mouth:"normal_talk" });`

b: Q--

(#act3a_after)

# act3a_after

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

h: Sai, ti avrei potuto credere... if you hadn't tried that a zillion times before.

h: You're the wolf who cried wolf.

```
bb({ eyes:"sad" });
```

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_harm"`

[](#act3_fork) `_.SPECIAL_ATTACK="harm"; Game.OVERRIDE_CHOICE_LINE=true`

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_alone"`

[](#act3_fork) `_.SPECIAL_ATTACK="alone"; Game.OVERRIDE_CHOICE_LINE=true`

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_bad"`

[](#act3_fork) `_.SPECIAL_ATTACK="bad"; Game.OVERRIDE_CHOICE_LINE=true`


# act3_fork

```
Game.clearText();
bb({body:"special_attack"});
sfx("charging");
Game.FORCE_CANT_SKIP = true;
```

(...1001)

```
Game.FORCE_CANT_SKIP = false;
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

h: You tried that too.

b: Umano, ti prego...

`hong({ eyes:"look_right" });`

h: Oh I'm *sorry* Big Pharma doesn't approve of my self-medication.

h: Look ^asshole^, we *all* have a way of shutting you the ^fuck^ up.

`hong({ body:"look_up", eyes:"look_up" });`

h: C'è chi si lancia nel lavoro.Some people throw themselves into work.

`hong({ body:"look_down", eyes:"look_down" });`

h: C'è chi si lancia nel sesso, nella droga, o aggiornando la pagina di Facebook.Some people throw themselves into sex, drugs, and refreshing their Facebook feed.

`hong({ body:"normal", eyes:"look_right" });`

h: C'è che si lancia in altre persone.Some people throw themselves into other people. 

`hong({ eyes:"angry" });`

h: Io mi lancerò in quella piscina.I'm going to throw myself into that swimming pool.

[Hai bevuto troppo, e siamo al SESTO PIANO](#act3_bad_1_harm)

[Cavolo, questo è il tuo ringraziamento?!](#act3_bad_1_insult) `bb({eyes:"angry"});`

[Ok, lo ammetto. Ho sbagliato tutto.](#act3_good_1) `bb({mouth:"sorry", eyes:"sorry_down"});`

# act3_bad_1_harm

b: Even if you land in the water, the surface tension will crack your ribs and give you a concussion *at the least!*

h: Eh.

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal", mouth:"angry", eyes:"angry" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

h: Ho visto su YouTube un tizio russo farlo, una volta.I saw a Russian guy do this on YouTube once.

(#act3_bad_2)

# act3_bad_1_insult

`hong({ eyes:"look_right" });`

h: Scusa, hai detto *grazie*?

`bb({ eyes:"angry" });`

b: This is exactly why I *exist!* Because humans can't be trusted to protect themselves!

b: Ti ho provato a salvare il ^culo^ per tutta la vita, e ora stai per-

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal", mouth:"angry", eyes:"angry" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

(#act3_bad_2)

# act3_good_1

`hong({ body:"laugh_1" })``

h: Eh.

`hong({ body:"laugh_2" })``

h: Ahahahah

`hong({ body:"laugh_3" })``

h: AHAHAHAHAHAH

```
bb({ eyes:"sorry"});
hong({ body:"yell_1", mouth:"yell", eyes:"blank" });
```

h: Oh WOW is that the biggest *^fuck^ing* understatement of the century!

`hong({ body:"yell_2" });`

h: Yeah, you rotting pile of blood-coated ^shit^! You messed the ^fuck^ up!

`hong({ body:"normal", mouth:"angry", eyes:"angry" });`

h: Any other remarks, Capitan Ovvio?

[But revenge on me isn't the answer!](#act3_good_1_fail_revenge) `bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });`

[But this time I'm *actually* right!](#act3_good_1_fail_harm) `bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });`

[I've hurt you.](#act3_good_2a)


# act3_good_1_fail_revenge

b: You need to have a healthier relationship with your emotions, rather than drown them wi--

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal", mouth:"angry", eyes:"angry" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

(#act3_bad_2)



# act3_good_1_fail_harm

b: Quindi per favore, metti giù la bottiglia e and-

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal", mouth:"angry", eyes:"angry" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

(#act3_bad_2)




# act3_bad_2

`bb({ eyes:"sad" });`

b: Ti prego... Non...

h: Your energy bar's looking awfully low there, wolf.

h: Fossi in te, sceglierei le tue prossime parole attentamente.

`bb({ eyes:"normal" });`

[Va bene. Non ti proteggerò più.](#act3_bad_2_jump) `bb({ mouth:"ignore", eyes:"ignore" });`

[Avevo sempre avuto ragione.](#act3_bad_2_right)

[Mi dispiace.](#act3_good_2b) `bb({mouth:"sorry", eyes:"sorry_down"});`


# act3_bad_2_jump

b: Allora, vai e salta. See what I care.

`hong({ eyes:"look_right", mouth:"normal", MOUTH_LOCK:true });`

h: ...

```
hong({ eyes:"less_angry", mouth:"normal" });
bb({ eyes:"ignore_oh_crap" });
```

h: Ok, allora. Alzati.

```
bb({ mouth:"normal", eyes:"oh_crap" });
Game.OVERRIDE_TEXT_SPEED = 2;
```

b: WAIT NO THAT WAS REVERSE PSYCHOLOGY YOU WERE SUPPOSED TO DO THE *OPPOSITE* OF WHAT I SA--

(#act3_bad_3)



# act3_bad_2_right

`bb({ eyes:"angry" });`

b: You *are* putting yourself in danger. Your so-called friends *are* using you. And *you* are using your so-called friends.

`bb({ eyes:"sad" });`

b: Quindi, per favore... perché non mi credi?!

h: Perché tu non hai mai creduto in *me*.

(#act3_bad_3)


# act3_bad_2_terrible

`bb({ eyes:"angry" });`

b: Other guard-wolves have humans who actually take time to patiently train them, to *learn* to work together,

b: Rather than hate the guard-wolves for trying to protect them! So why can't you jus--

`bb({ eyes:"normal" });`

h: Risposta sbagliata, ^cazzo^.

(#act3_bad_3)



# act3_bad_3

```
music(null);
hong({body:"drink"});
bb({body:"attacked"});
publish("bb_STOP_VIBRATING");
attackBB("100p");
```

(...2000)

```
hong({ body:"normal", mouth:"normal", eyes:"normal" });
bb({ body:"dead" });
```

(...999)

h: *"The only thing to fear is fear itself."*

`hong({ body:"look_up", mouth:"happy", eyes:"blank" });`

h: *"Stai senza pensieri!"*

`hong({ body:"normal", mouth:"normal", eyes:"normal" });`

h: Lo dicono tutti i saggi contemporanei: le emozioni negative sono *cattive*!

`hong({ eyes:"less_angry" });`

h: Beh, sennò non si chiamavano *negative*!

b: Umano... Per favore...

`hong({ eyes:"normal" });`

h: Un po' di tempo fa dissi: “Voglio solo liberarmi di tutto questo dolore.”

h: Ho ottenuto quello che volevo. Non sento più dolore, o paura, o ansia...

h: Non sento più nulla.

`_.a3_ending = "jump";`

(#act3_end)



# act3_good_2a

`bb({mouth:"sorry", eyes:"sorry_down"});`

b: I was so obsessed with making sure nothing else hurt you, that I didn't realize *I* was creating the hurt.

```
bb({ eyes:"sorry"});
hong({ body:"yell_2", mouth:"yell", eyes:"blank" });
```

h: NO. ^MERDA^.

`hong({ body:"yell_1" });`

h: ^CAZZO^. Ti ci è voluto così tanto per capirlo, finalmente?!

`hong({ body:"cry", mouth:"cry", eyes:"blank" });`

h: Ci avresti fatto risparmiare un sacco di guai, grandissimo ^bastardo^ peloso. Perché non l'hai capito prima?...

`_.apologized_for_hurt = true;`

(#act3_good_2q)



# act3_good_2b

`hong({ body:"normal", mouth:"angry", eyes:"look_right" });`

h: Ti *dispiace*...

`hong({ eyes:"angry", MOUTH_LOCK:true });`

h: ...

h: Ti dispiace per *cosa*?

(#act3_good_2q)


# act3_good_2q

`bb({mouth:"sorry", eyes:"sorry"});`

{{if _.apologized_for_hurt}}
(#act3_good_2q_already_apologized)
{{/if}}

{{if !_.apologized_for_hurt}}
(#act3_good_2q_not_already_apologized)
{{/if}}


# act3_good_2q_already_apologized

`hong({ body:"normal", mouth:"angry", eyes:"less_angry" });`

[Mi dispiace di non averti protetto.](#act3_good_3_protector)

[Mi dispiace di non averti rispettato.](#act3_good_3_respect)

[Mi dispiace.](#act3_good_4)


# act3_good_2q_not_already_apologized

`hong({ body:"normal", mouth:"angry", eyes:"angry" }, 0);`

[Mi dispiace di avere un terribile umano!](#act3_bad_2_terrible) `bb({mouth:"normal", eyes:"normal"})`

[Mi dispiace di non averti rispettato.](#act3_good_3_respect)

[Mi dispiace di averti ferito.](#act3_good_3_hurt)



# act3_good_3_protector

`bb({eyes:"sorry_down"});`

b: It's my duty to warn you against *real* danger, but I kept barking at cars and the mailman.

`bb({eyes:"sorry_up"});`

b: Barking at shadows. Barking so much.

`bb({eyes:"sorry"});`

b: It only makes sense that you'd want to muzzle me.

`bb({eyes:"sorry_down"});`

b: Mi dispiace.

(#act3_good_4)



# act3_good_3_respect

`bb({eyes:"sorry_down"});`

b: Dovevo essere il *tuo* fedele cane da guardia, ma mi sono comportato come se tu dovessi obbedire a *me*.

`bb({eyes:"sorry_up"});`

b: There's a difference between a protector and a prison warden, e ho esagerato.

`bb({eyes:"sorry_down"});`

b: Mi dispiace.

(#act3_good_4)



# act3_good_3_hurt

`bb({eyes:"sorry_down"});`

b: I was so obsessed with trying to protect you from being hurt, I never stopped to realize *I* was hurting you.

`bb({eyes:"sorry_up"});`

b: Non sono stato un bravo cagnolino.

`bb({eyes:"sorry_down"});`

b: Mi dispiace.

(#act3_good_4)


# act3_good_4

```
music(null,{fade:3});
hong({ eyes:"less_angry", MOUTH_LOCK:true },0);
```

h: ...

```
hong({ body:"stop", mouth:"stop", eyes:"blank" });
```

h: Sì, beh, era comunque un'idea assurda.

h: I only did this to mess you up, and, well, I messed you up.

h: Facciamo che siamo pari, ok?

```
bb({ mouth:"sorry", eyes:"sorry" });
bb({ MOUTH_LOCK:true });
```

b: ...

b: Ok.

h: Ok.

n: *PAREGGIO*

`_.a3_ending = "walkaway";`

(#act3_end)









# act3_end

```
Game.clearText();
publish("act3-in");
publish("hp_hide");
Game.FORCE_CANT_SKIP = true;
```

{{if _.a3_ending=="walkaway"}}
(#act3_walkaway)
{{/if}}

{{if _.a3_ending=="jump"}}
(#act3_jump)
{{/if}}






# act3_walkaway

```
publish("start-walkaway-anim");
Game.WORDS_HEIGHT_BOTTOM = 205;
```

(...3501)

```
sfx("bottle_toss");
publish('hong-next');
publish("act3",["roofhunter",7]);
```

(...667)

```
publish("act3",["dd",4]);
publish("act3",["roofhunter",26]);
publish('hong-next');
sfx("concrete_step1");
```

(...667)

```
publish('hong-next');
sfx("concrete_step2");
```

(...667)

```
publish('hong-next');
publish("act3",["roofhunter",27]);
```

`Game.FORCE_CANT_SKIP = false;`

r: Oh, *ma dai*. Dopo tutto quello che ti ha fatto l'animale, ti *arrendi* così?

r: Che problema c'è, giovane? Hai *paura*?

```
publish('hong-next');
publish("act3",["roofhunter",26]);
```

h2: Sì.

h2: Ho paura.

`publish('hong-next')`

h2: E va bene così!

`publish('hong-next')`

h2: Va bene avere paura.

`publish('hong-next')`

(...500)

```
Game.clearText();
Game.FORCE_CANT_SKIP = true;
```

(...1167)

```
publish('hong-next');
```

(...833)

```
publish('hong-next');
sfx("rustle2");
```

(...1333)

```
publish('hong-next');
publish("act3",["dd",5]);
publish("act3",["roofhunter",31]);
sfx("concrete_step4");
```

(...667)

```
publish('hong-next');
sfx("concrete_step1");
```

(...667)

```
publish('hong-next');
sfx("door");
```

(...1333)

```
publish('hong-next');
sfx("concrete_step2");
```

(...501)

```
publish('hong-next');
Game.FORCE_CANT_SKIP = false;
sfx("lock_door");
publish("act3",["roofhunter",32]);
```

(...2001)

```
publish("act3",["roofhunter",33]);
```

r: Ma mi ha chiuso a chiave?

```
Game.clearAll();
_.INJURED = false;
Game.WORDS_HEIGHT_BOTTOM = -1;
```

(...2000)

(#act4)




# act3_jump

```
publish("start-jump-anim");
Game.FORCE_TEXT_Y = 300;
```

(...2001)

```
publish('hong-next');
sfx("bottle_toss");
```

(...833)

```
sfx("concrete_step1");
sfx("claps");
publish('hong-next');
publish("act3",["dd",4]);
publish("act3",["roofhunter",28]);
```
(...125)

`publish("act3",["roofhunter",29]);`

(...125)

`publish("act3",["roofhunter",28]);`

(...125)

`publish("act3",["roofhunter",29]);`

(...125)

```
sfx("concrete_step2");
publish('hong-next');
publish("act3",["roofhunter",28]);
```

(...125)

`publish("act3",["roofhunter",29]);`

(...125)

`publish("act3",["roofhunter",28]);`

(...125)

`publish("act3",["roofhunter",29]);`

(...125)

```
sfx("concrete_step3");
publish('hong-next');
publish("act3",["dd",5]);
publish("act3",["roofhunter",34]);
```

(...1167)

```
sfx("rustle2");
publish('hong-next');
```

(...1001)

`publish('hong-next')`

b: no...

(...501)

`Game.clearText();`

`publish('hong-next')`

(...1333)

```
sfx("quack");
publish('hong-next');
```

(...1333)

`publish('hong-next')`

b: no no no

(...501)

`Game.clearText();`

`publish('hong-next')`

(...2001)

```
sfx("rustle2");
publish('hong-next')
```

(...501)

```
sfx("concrete_step1");
publish('hong-next');
publish("act3",["dd",4]);
publish("act3",["roofhunter",30]);
```

(...167)

```
sfx("concrete_step2");
publish('hong-next');
```

(...167)

```
sfx("concrete_step3");
publish('hong-next');
publish("act3",["dd",2]);
publish("act3",["roofhunter",15]);
```

(...167)

```
sfx("bottle_slip");
publish('hong-next');
publish("act3",["dd",3]);
publish("act3",["roofhunter",16]);
```

(...833)

```
sfx("rustle");
publish('hong-next');
```

(...167)

`publish('hong-next')`

(...167)

```
publish('hong-next');
Game.FORCE_TEXT_Y = 325;
Game.OVERRIDE_FONT_SIZE = 50;
```

b: NO!

(...400)

```
Game.WORDS_HEIGHT_BOTTOM = -1;
Game.FORCE_TEXT_Y = -1;
Game.clearText();
publish("act4-injury-show");
publish("hide_tabs");
```

(...2000)

```
sfx("hospital1");
publish("act4-injury", [1]);
```

(...4000)

```
stopAllSounds();
publish("act4-injury", [0]);
```

(...2000)

```
sfx("hospital2");
publish("act4-injury", [2]);
```

(...4000)

```
stopAllSounds();
publish("act4-injury", [0]);
```

(...2000)

```
sfx("hospital3");
publish("act4-injury", [3]);
```

(...8000)

```
stopAllSounds();
publish("act4-injury", [0]);
```

(...5500)

`_.INJURED = true;`

(#act4)
