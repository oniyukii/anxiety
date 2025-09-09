# intro

`SceneSetup.intro();`

# intro-play-button

(...51)

```
_.PLAYED_BEFORE = !!window.localStorage.continueChapter;
```

{{if !_.PLAYED_BEFORE}}
`Game.OVERRIDE_FONT_SIZE=30;`
{{/if}}

{{if !_.PLAYED_BEFORE}}
[#play1# GIOCA! #play2#](#intro-start) `publish("intro-to-game-1"); Game.OVERRIDE_CHOICE_LINE=true;`
{{/if}}

{{if _.PLAYED_BEFORE && window.localStorage.continueChapter=="act2"}}
[_CONTINUA_: La festa](#act2) `publish("LOAD_GAME", ["act2"]); Game.OVERRIDE_CHOICE_LINE=true;`
{{/if}}

{{if _.PLAYED_BEFORE && window.localStorage.continueChapter=="act3"}}
[_CONTINUA_: L'altra festa](#act3) `publish("LOAD_GAME", ["act3"]); Game.OVERRIDE_CHOICE_LINE=true;`
{{/if}}

{{if _.PLAYED_BEFORE && window.localStorage.continueChapter=="act4"}}
[_CONTINUA_: L'altro panino](#act4) `publish("LOAD_GAME", ["act4"]); Game.OVERRIDE_CHOICE_LINE=true;`
{{/if}}

{{if _.PLAYED_BEFORE && window.localStorage.continueChapter=="replay"}}
`Game.OVERRIDE_FONT_SIZE=30;`
{{/if}}

{{if _.PLAYED_BEFORE && window.localStorage.continueChapter=="replay"}}
[#play1# RIGIOCA! #play2#](#intro-start) `publish("intro-to-game-1"); Game.OVERRIDE_CHOICE_LINE=true;`
{{/if}}

{{if _.PLAYED_BEFORE}}
[Seleziona capitolo](#chapter-select) `Game.OVERRIDE_CHOICE_LINE=true;`
{{/if}}

[(Note di contenuti)](#intro-play-button) `Game.OVERRIDE_CHOICE_LINE=true; publish('show_cn');`

# chapter-select

`publish("HACK_chselect");`

[I. Il panino](#intro-start) `publish("HACK_chselect_end"); publish("intro-to-game-1"); Game.OVERRIDE_CHOICE_LINE=true;`

[II. La festa](#act2) `publish("HACK_chselect_end"); publish("LOAD_GAME", ["act2"]); Game.OVERRIDE_CHOICE_LINE=true;`

{{if window.localStorage.act3}}
[III. L'altra festa](#act3) `publish("HACK_chselect_end"); publish("LOAD_GAME", ["act3"]); Game.OVERRIDE_CHOICE_LINE=true;`
{{/if}}

{{if !window.localStorage.act3}}
[III. L'altra festa]()
{{/if}}

{{if window.localStorage.act4}}
[IV. L'altro panino](#act4) `publish("HACK_chselect_end"); publish("LOAD_GAME", ["act4"]); Game.OVERRIDE_CHOICE_LINE=true;`
{{/if}}

{{if !window.localStorage.act4}}
[III. L'altro panino]()
{{/if}}

{{if window.localStorage.credits}}
[V. Riconoscimenti](#to-credits) `publish("HACK_chselect_end"); Game.OVERRIDE_CHOICE_LINE=true;`
{{/if}}

{{if !window.localStorage.credits}}
[V. Riconoscimenti]()
{{/if}}

[(main menu)](#intro-play-button) `publish("HACK_chselect_end"); Game.OVERRIDE_CHOICE_LINE=true;`

# to-credits

`stopAllSounds();`

(...101)

(#credits)

# intro-start

(...500)

`clearText()`

n3: Ciao! Questo non è proprio un "gioco", ma una storia interattiva. Buona lettura, perdente!

n3: Prima di iniziare, imposta la *tua* preferenza di lettura!

`publish("show_options_bottom")`

# intro-start-2

n3: Ottimo! Nota: puoi modificare le impostazioni con l'icona ⚙ in basso. Inoltre, il gioco si salverà in automatico ad ogni capitolo!

n3: E adesso, iniziamo la nostra storia...

`clearText()`

(...1000)

`publish("intro-to-game-2")`

n2: QUESTO È UN UMANO

(...600)

`clearText()`

(...300)

`publish("intro-to-game-3")`
