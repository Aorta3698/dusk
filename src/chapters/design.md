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
- Fair workload for each finger

Coming from Canary, I'd like to focus on keeping its low scissors and 2u SFS, while optimizing for SFS and keeping an eye on SFB.

`Dusk` was designed with info obtained with corpus made out of MonkeyType and Typeracer quotes (duplicates removed), with some SHAI corpus sprinkled in.

## Vowel Block
I decided to go with the popular vowel block
```
~ ~ ~ ~ ~  ~ ~ O U .
~ ~ ~ ~ ~  ~ ~ A E I
~ ~ ~ ~ ~  ~ ~ ~ / ,
        ~
```
as `EO` is the primary source of SFS on Canary and `OU` `AEI` vowel block is commonly agreed upon to be the most balanced vowel block choice in modern days.
Having `I` alone on the pinky for the `.I,` stack.

Why vowel block? because vowels don't go well with most letters, but they go relatively well with each other.

If you type `./` or `../` often, you may want to swap `.,`.

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
I like the idea of having `N` on the pinky because they promote inroll with `S`, `T`, `C` and tend to be have lower redirection and scissors especially now that `R` is gone (usually `N` pinky layouts end up with `BR` scissor like in `Graphite` and `Gallium`).

`N` doesn't interact with `B` much and with a low-usage key `Z`, `BNZ` goes to pinky. `X` wasn't chosen out of concerns for the interactions with the columns that follow below.

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

#### Wait a minute!
You may think, "wait a minute! but that creates `NV` scissor and awkward `DV` !". Yes, I hear you, so there is another variant [`dusk-vq`](./layout.md#dusk-vq) that addresses this concern.

What's the trade-off?

Pros:
- no `NV` scissor (`involve`)
- no `DV` (`advice`)
- no `b_v` skip scissor (`above`)
- no `f_v` 2u SFS (`favorite`)

Cons:
- `w_v` 2u SFS (`however`)
- `g_v` 2.23u SFS (`give`)
- `v__g` 2.23u SFS (`loving`)
- `rv` and `v_r` may be weird for some (`service` and `very`).
- 6 keys to look after for left index.

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

- `W` is under `Y` because `W_Y` is common, in addition to `YW` SFB. It is not above `Y` because `W_T`, `W__T`, `W__K`, `TW` and `WR` all feel awful. I am okay with `P_W` or `W_P` 2.24u SFS as they are rare.

- `P` takes the last good spot and creates `PY` and `YP` alts.

#### I don't want to alt!

If you don't want to alt/slide `CY`, `PY`, `YP`, `GY`, and `WY`, and get deeply annoyed with them. May I suggest that you do
```
B F D P ~  ~ ~ O U .
N S T C Y  M H A E I
Z V K G W  ~ L Y / ,
        R
```
Now you have 2 `Y` that you can choose to use according to the words in question.

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

This results in 0.10% lower SFB and 0.29% higher SFS on MonkeyRacer corpus. 
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

It results in 0.04% lower SFB and 0.01% lower SFS on Monkeyracer corpus, but it increases redirection by 0.59% on according to Cmini, attributed to `t's` and `n't`. Additionally, both `'t` and `t'` do not feel good to me.
```
B F D P '  Q J O U .
N S T C Y  M H A E I
Z V K G W  X L ~ / ,
        R
```
#### Alternative 3
Put `'` at both empty spots. Use the bottom `'` for `'m` and `'ll`.
```
B F D P Q  J ' O U .
N S T C Y  M H A E I
Z V K G W  X L ' / ,
        R
```


### Last Spot Options
It's free real estate. I decided to put underscore `_` there because I code in `C++` and `Rust` often. 

Here are some ideas:
- `;` 
- `Y`
- `'`
- Repeat Key (creates `LL` outroll)

```
B F D P Q  J ' O U .
N S T C Y  M H A E I
Z V K G W  X L _ / ,
        R
```

## Final Adjustment
One user of Dusk, `brownfoxjumps`, mentioned that he was using dusk with `BZ` swap. This got me thinking - as `Dusk` it is now, words like `above`, `back`, `break`, `obvious`, and `keyboard` all require whole hand movement due to (skipgram) scissors. If `BZ` is swapped, then the only key that would be of concern is the top ring key `F`, but `B` and `F` don't really interact with each other much at all - except for the word `before`. `b_d` and `prob-` still don't require hand movement and feel fine. I decided that swapping `BZ` is worth it.

```
Z F D P Q  J ' O U .
N S T C Y  M H A E I
B V K G W  X L _ / ,
        R
```

With `Z` up there, it now raises the question of whether it is worth it to swap `XZ`. Personally, I think it is worth it because 2 out of the 3 reasons that I chose `Z` instead of `X` were that `XP` is awkward and the `f_x` scissor. With these two reasons no longer applicable, I think it is worth trading the rare 2u pinky SFS (`box`) for taking 0.01% lower SFB and 0.05% lower SFS (SHAI corpus) off from the finger with the highest SFS and SFB, and that sweet `XP` inroll (`expect`, `experience`).

```
X F D P Q  J ' O U .
N S T C Y  M H A E I
B V K G W  Z L _ / ,
        R
```

### What about `FV` swap?
Some of you may be wondering: why not the following layout? Doesn't it address `b_f` and `dv` while not losing out much (`g_v` but it is no big deal)?

```
Z V D P Q  J ' O U .
N S T C Y  M H A E I
B F K G W  X L _ / ,
        R
```
I toyed with this idea for a while and came to the conclusion that it is not worth it because of `f_nd`, which is quite a lot more common than `dv` on dusk while feeling worse than it.

Summary:

#### Pros
- `dv` roll
- `b_f` same row

#### Cons
- `f_nd` skipgram redirect 2 row jump
- `xz` forced swap or getting `f_x` skipgram scissor
- `bv`/`b_v` 2 row jump
