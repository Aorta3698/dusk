# Design

<!-- toc -->

## Goals
`Dusk` was designed with these goals in mind:
- Roll over Alternation
- Low scissors
- Low 2u SFS (including some fast `X__Y`)
- Low SFS
- Low SFB
- Low finger speed
- Low usage for pinky and ring bottom keys
- No finger gets overworked

Low SFS takes slight priority over low SFB with respect to a ratio, and low 2u SFS and scissors, including half scissors, take priority over both SFS and SFB.

## Vowel Block
I decided to go with the popular vowel block
```
~ ~ ~ ~ ~  ~ ~ O U .
~ ~ ~ ~ ~  ~ ~ A E I
~ ~ ~ ~ ~  ~ ~ ~ / ,
        ~
```
as it as commonly agreed upon to be the most balanced vowel block choice.
Having `I` alone on the pinky for the `.I,` stack.

Why vowel block? because vowels don't go well with most letters, but they go relatively well with each other.

Feel free to swap `.,` if you prefer that way.

## Consonants

### `LHM`
To avoid `RL` SFB, I decided to put `R` on a thumb key (as opposed to the `RN` stack as seen in `Kuntum`). `L` doesn't really go well with any other letter except for `H` and `M`, but `L_M` and `M_L` are both somewhat common, which leads to `LHM` stack having high 2u SFS if its on a non-index column, so `LHM` goes to index with `M` taking the inner spot, just like in Canary. If you are more bothered by LSB than 2u SFS, it would be wise to move `M` to the top.
```
~ ~ ~ ~ ~  ~ ~ O U .
~ ~ ~ ~ ~  M H A E I
~ ~ ~ ~ ~  ~ L ~ / ,
        R
```
### `DTK`
`T` index commonly leads to high SFS in my experience playing around with layouts for the past few months, so I settled on `DTK` stack, which is a good load for the middle finger to handle.

```
~ ~ D ~ ~  ~ ~ O U .
~ ~ T ~ ~  M H A E I
~ ~ K ~ ~  ~ L ~ / ,
        R
```
### `BNZ`
I like the idea of having `N` on the pinky because they tend to be quite non-offensive with low redirection and scissors especially now that `R` is gone (usually `N` pinky layouts end up with `BR` scissor like in `Graphite` and `Gallium`).

`N` doesn't interact with `B` much and with a low-usage key `Z`, `BNZ` goes to pinky.

```
B ~ D ~ ~  ~ ~ O U .
N ~ T ~ ~  M H A E I
Z ~ K ~ ~  ~ L ~ / ,
        R
```
### `FSV`
`ST` in-roll sounds like a good idea and `S` doesn't have good letters to partner, so I decided on `FSV` stack for the ring finger.
```
B F D ~ ~  ~ ~ O U .
N S T ~ ~  M H A E I
Z V K ~ ~  ~ L ~ / ,
        R
```
### `PCGWY`
`Y` is yet another problematic letter as it creates `CY`, `PY`, `GY` SFBS and `W_Y` is common enough that I'd like `WY` to be 1u apart. 
I decided on
```
B F D P ~  ~ ~ O U .
N S T C Y  M H A E I
Z V K G W  ~ L ~ / ,
        R
```
because:
- I want `NG` to be a nice roll and a good `G_T` (`-ing`, `-ght`, `get`, `got`).
- `C` is usually more common, so it is on the homerow.
- `Y` is there for the ease of alting `CY`, `PY`, `YP` and (optionally) `GY`.
- `W` is under `Y` because `W_Y` is common, in addition to `YW` SFB. It is not above `Y` because `W_T`, `W__T`, `W__K`, `TW` and `WR` all feel awful. I am okay with `P_W` or `W_P` 2.5u SFS as they are rare.
- `P` takes the last good spot and creates `PY` and `YP` alts.

### `QJX`
- `J` goes well with vowel inner top spot because `JU` accounts for most of `J` appearances.
- `X` does not go well with `C` and `P` (`excel`, `expect`), so it goes to vowel inner bottom spot.
- `Q` takes the last remaining index spot at consonants side.
```
B F D P Q  J ~ O U .
N S T C Y  M H A E I
Z V K G W  X L ~ / ,
        R
```

### Quote Symbol `'`
Other layouts commonly have `OA'` stack on the middle finger, but after using other layouts that have this stack, I've come to dislike it. Here is why:
- `You'` feels like 2u SFB even if it is 2u SFS. For me, `ou` is a roll, so my middle finger tends to not leave for `'` until after `u` has been typed.
- `don't` and `won't` feel just awful with how common they are.
- Additionally, `a_'` is common too (`that's`, `can't`, `what's`).

For the aforemetioned reasons, I decided to go with
```
B F D P Q  J ' O U .
N S T C Y  M H A E I
Z V K G W  X L ~ / ,
        R
```
with the intention to alt `'m` and `'ll`, both of which are doable for my columnar keyboard.  If you do not want to do `'ll` alt, I think it is still preferable over `OA'` stack. (I do not believe `'ll` alt is feasible on rowstag keyboard).

It does create `h_'` SFS, but it is about as common as `a_'`.

#### Alternative 1
Embrace the `OA'` stack like the layout below shows - all the pros and cons have been explained above.

You may want to swap `J~`.
```
B F D P Q  J ~ O U .
N S T C Y  M H A E I
Z V K G W  X L ' / ,
        R
```
#### Alternative 2
Swap `QJ'`.

Keep in mind that it creates
- `Y'` SFB (`They'`)
- `W_'` SFS (`We'`)
- `DN'` redirection (`don't`)
- `C__'` SFS (`can't`)

It results in roughly the same SFB or SFS on either SHAI or Monkeyracer, but it increases redirection by 0.58% on Monkeyracer corpus according to Cmini.
```
B F D P '  Q J O U .
N S T C Y  M H A E I
Z V K G W  X L ~ / ,
        R
```


### The Last Spot
It's free real estate. I decided to put underscore `_` there because I code in `C++` and `Rust` often. You can put `;` there if you'd like, or anything really.

```
B F D P Q  J ' O U .
N S T C Y  M H A E I
Z V K G W  X L _ / ,
        R
```
