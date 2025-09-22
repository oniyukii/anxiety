# intro

`SceneSetup.intro();`

# intro-play-button

[<div class="mini-icon" pic="play1"></div> GIOCA! <div class="mini-icon" pic="play2"></div>](#intro-start) `publish("intro-to-game-1"); Game.OVERRIDE_CHOICE_LINE=true;`

# intro-start

(...500)

`clearText()`

n3: Ops

`publish("show_options_bottom")`

# intro-start-2

`clearText()`

(...1000)

`publish("intro-to-game-2")`

n2: QUESTO È UN UMANO

(...600)

`clearText()`

(...300)

`publish("intro-to-game-3")`

# act1

`SceneSetup.act1();`

(...300)

n: E QUESTA È LA SUA ANSIA

n: _TU_ SEI L'ANSIA

[Stiamo pranzando da soli! Di nuovo!](#act1a_alone)

[Non stiamo facendo nulla mentre mangiamo!](#act1a_productive)

[Il pane bianco fa male!](#act1a_bread)

# act1a_alone

`bb({mouth:"small", eyes:"narrow"})`

b: Lo sapevi che la solitudine cronica è tanto letale quanto fumare 15 sigarette al giorno?

`Game.OVERRIDE_TEXT_SPEED = 2;`

`bb({mouth:"normal", eyes:"normal_right"})`

b: (Holt-Lunstad et al, 2010, PLoS Medicine)

`hong({mouth:"0_neutral", eyes:"0_annoyed"})`

h: Ehm, grazie per aver citato le fonti, ma--

`Game.OVERRIDE_TEXT_SPEED = 2;`

`bb({body:"fear", mouth:"normal", eyes:"fear"})`

b: Significa che se non usciamo con qualcuno *adesso*, noi--

`bb({body:"panic"})`

b: MORIREMOOOOOOOOOOOOO

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("20p", "alone");
publish("hp_show");
```

(...2500)
