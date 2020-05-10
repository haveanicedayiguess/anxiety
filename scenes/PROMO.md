# intro

`SceneSetup.intro();`

# intro-play-button

(...51)

[PLAY!](#intro-start) `publish("intro-to-game-1"); Game.OVERRIDE_CHOICE_LINE=true;`

# intro-start

(...500)

`clearText()`

n3:  Så, inden vi begynder, hvordan kunne *du* tænke dig at læse?

`publish("show_options_bottom")`

# intro-start-2

n3:  Lad os begynde på vores fortælling...

```
publish("hide_tabs");
clearText();
```

(...1000)

`publish("intro-to-game-2")`

n2: DET HER ER ET MENNESKE

(...600)

`clearText()`

(...300)

`publish("intro-to-game-3")`

# act1

```
SceneSetup.act1();
publish("hide_tabs");
music('battle', {volume:0.5});
```

(...300)

n: OG DET HER ER MENNESKETS ANGST

n:  _DU_ ER ANGSTEN

(#act1_normal)


# act1_normal

```
hong({body:"putaway"});
sfx("rustle");
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Nej. Nej, nope, jeg lytter ikke. Tjekker min telefon.

```
sfx("rustle2");
hong({body:"phone1", mouth:"neutral", eyes:"neutral"})
```

n: DIT JOB ER AT BESKYTTE DIT MENNESKE FRA *FARE*

`bb({eyes:"look", mouth:"small_lock", body:"fear"})`

b: Gisp! Du scroller dit liv væk på Twitter! Igen!

```
bb({eyes:"normal", mouth:"normal", body:"normal"});
hong({eyes:"annoyed"});
```

h: Jeg undrer mig da over hvorfor jeg ikke lytter til mine tanker lidt oftere.

`hong({eyes:"neutral"});`

n: HURTIGT, ADVAR DEM OM EN *FARE!*

```
bb({eyes:"look"});
```

[Åh nej, se den forfærdelige historie i nyhederne!](#act1d_news)

[Åh nej, er den tweet faktisk om *os?*](#act1d_subtweet)

[Hey, en GIF af en kat der drikker mælk](#act1d_milk)

# act1d_milk

`hong({mouth:"smile", eyes:"surprise"});`

h: Heh, det er cute, det--

```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b: KATTE KAN IKKE TÅLE MÆLK OG VI ER FORFÆRDELIGE MENNESKER FOR AT KUNNE LIDE DYREMISHANDLING

(...200)

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
attack("20p", "bad");
publish("hp_show");
```



