# FAQ

<!-- toc -->

## Compare Canary to Dusk is not fair!
Yes, I agree, but I used to main `Canary-ortho`, it makes sense for me to compare them.

Feel free to compare `Dusk` against other thumb layouts such as `Pine-y`, `Sturdy-thumbn`, `Aptmak`, `Bunya`, or `Chrono`.

`Chrono` (another layout of mine) beats `Dusk` for having even lower SFS, low LSB, and no inner corner key like `W` in `Dusk`, but in exchange getting `LK` ring-middle full scissor, `RL` SFB, and `BR` scissor.

```
chrono
  b l d p z  q w o u .
  n r t h y  g c a e i
  x j k f v  ' m ; / ,
        s                   

MONKEYRACER:
  Alt: 30.72%
  Rol: 44.80%   (In/Out: 26.31% | 18.49%)
  One:  1.95%   (In/Out:  0.71% |  1.24%)
  Rtl: 46.75%   (In/Out: 27.02% | 19.73%)
  Red:  3.67%   (Bad:     0.38%)

  SFB: 0.53%
  SFS: 3.67%    (Red/Alt: 0.98% | 2.69%)

  LH/RH: 49.94% | 50.06%
```
## I hate where ' is!
Explore these options:
- [Option 1](/src/chapters/design.md#alternative-1)
- [Optoin 2](./design.md#alternative-2)
- [Option 3](./design.md#alternative-3)

## I hate where `V` is!
Consider [`Dusk-qvz`](./layout.md#dusk-qvz).

## Why not swap 2 index block?
- It increases alternation by a whopping 4% to 32.XX% on Cmini with Monkeyracer corpus, which is too high for my taste.
- `OW` and `WO` would suck. I consider that scissors. Swapping `W` and `Q` won't help because then `WA` would suck.
- The intended `CY`, `YC`, `PY`, `YP` alts would be less feasible. Think words like `happy` or `privacy`.

## Why not swap `X` and `Z` for lower SFB and SFS?
- `F_X` is a skip full pinky-ring scissor (`fix`).
- `B_X` is a 2u pinky SFS (`unboxing`).
- `XP` is a bit awkward (`expect`).
- At the end of the day, stats isn't everything. Comfort should come first.

## How much worse is vowel thumb space and can I use thumb R with vowel thumb?
It is commonly known that space should be pressed with the consonant thumb because it has lower redirection and higher roll, and so why is the thumb `R` in `Dusk` on the consonant side?

The reason is simple - thanks to `a200` analyzer, I've come to the conclusion that even after considering the extra 0.52% redirection incurred by vowel space thumb, having `R` on the consonant thumb as opposed to the vowel thumb leads to approximately 3.87% lower redirection overall.

But then you may wonder: Is the redirection caused by thumb even real? How come that I have not felt any space redirection?

For me at least, after having tried `Dusk` with vowel thumb `R` for a few days, most redirection involving `R` is just as good, if not better than, the redirection involving index finger, but with one exception: when index `L` is also involved. Take the word `earlier` for example, that word just feels bad to type with vowel thumb `R`.

## What is the True SFB if I alt and slide?
If you 
- Alt `PY`, `YP`, `CY`, `'M`, and `'L`. 
- Slide `UE`, `OA`, `HL`, `YW`, and `FS`.

then SFB is almost none, leaving really only `GY`, `LM`, `I.`, and `I,`. None of which is common (unless you type `almost` a lot).

## I despise alting, can I re-arrange index letters?
Yes - arrange them how you like them!

## Can I use `Dusk` on a rowstag keyboard?
It is possible to do so with wide mod, but `Dusk` is designed for colstag keyboards, so I can't say the experience would be good. You may or may not want to re-arrange some index keys.

## Is Dusk good for e200 on MonkeyType?
It is :D

It doesn't have any SFB (0.00%) on e200 and with remarkably low SFS as well.
```
dusk
  b f d p q  j ' o u .
  n s t c y  m h a e i
  z v k g w  x l _ / ,
          r                 

ENGLISH-200:
  Alt: 30.73%
  Rol: 50.11%   (In/Out: 21.60% | 28.51%)
  One:  1.34%   (In/Out:  0.67% |  0.67%)
  Rtl: 51.45%   (In/Out: 22.27% | 29.18%)
  Red:  3.79%   (Bad:     0.22%)

  SFB: 0.00%
  SFS: 3.34%    (Red/Alt: 1.56% | 1.78%)

  LH/RH: 47.04% | 52.96%  
```

## `W` position... Really?
There is actually another version of Dusk: `Dusk_optimized`.

To get rid of `W` inner key, `Dusk_optimized` moved `P` to be with `BN`, and in doing so, it gets rid of the inner corner key and achieves even lower SFB and SFS. However, the cost of it is a whopping 1.41% increase in half scissors according to Keysolve.

I hesitate to recommend `Dusk_optimized` for the following reasons:

- Words like `prob`, `problem`, `public` being 2 row ring jump (much more freq than `f_v` or `f__v` on `Dusk`).

- There are some interaction with `P` and `K` such as `park` and `speak`.

- Interaction between `W` and `K`: `know`, `weak`, `woke` (`know` alone would be a deal breaker for me).

- Frequent `nk` half scissor and `w_t`, `w__t` skip half scissor.

- `nf` being out-roll scissor (I found pinky-ring scissor better as in-roll).

Swapping `WG` addresses some of the concerns above, but you get worse `ng` and `g_t`.

```
dusk_optimized
  f p d w q  j ' o u .
  s n t c y  m h a e i
  z b k g v  x l _ / ,
          r                   

MONKEYRACER:
  Alt: 28.31%
  Rol: 47.97%   (In/Out: 20.42% | 27.55%)
  One:  1.67%   (In/Out:  0.63% |  1.04%)
  Rtl: 49.64%   (In/Out: 21.06% | 28.58%)
  Red:  3.42%   (Bad:     0.39%)

  SFB: 0.36%
  SFS: 3.68%    (Red/Alt: 1.07% | 2.62%)

  LH/RH: 46.90% | 53.10%
```

## How did you make the figures in [Layout](./layout.md)?
It is from [here](https://keymap-drawer.streamlit.app/) with the following setting:
```
layout:
  qmk_keyboard: chocofi
  #qmk_layout: LAYOUT_split_3x5_2
layers:
  DEF:
    - [B, F, D, P, W, J, "'", O, U, .]
    - [N, S, T, C, Y, M, H, A, E, I]
    - [Q, Z, K, G, V, X, L, "_", /, ","]
    - {}
    - {t: R}
    - {}
    - {}
    - {t: Space}
    - {}

```
