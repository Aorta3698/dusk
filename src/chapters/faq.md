# FAQ

<!-- toc -->

## Compare Canary to Dusk is not fair!
Yes, I agree, but I used to main `Canary-ortho`, it makes sense for me to compare them.

For comparison with other thumb layouts, check out [Comparison](./cmp.md).

## I hate where ' is!
Explore these options:
- [Option 1](./design.md#alternative-1)
- [Optoin 2](./design.md#alternative-2)
- [Option 3](./design.md#alternative-3)

## I hate where `V` is!
Consider [`Dusk-qv`](./layout.md#dusk-qv).

## I hate `Y` due to SFBs
Explore [this option](./design.md#i-dont-want-to-alt).

## Why not swap 2 index block?
- It increases alternation by a whopping 4% to 32.XX% on Cmini with Monkeyracer corpus, which is too high for my taste.

- `OW` and `WO` middle-index full stretch would suck. Swapping `W` and `Q` won't help because then `WA` would suck.

- The intended `CY`, `YC`, `PY`, `YP` alts would be less feasible. Think words like `happy` or `privacy`.

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

## Can I re-arrange index letters?
Yes - arrange them how you like them!

## Can I use `Dusk` on a rowstag keyboard?
It is possible to do so with wide mod, but `Dusk` was designed for colstag keyboards, so I can't say the experience would be good. You may or may not want to re-arrange some letters.

## Is Dusk good for e200 on MonkeyType?
It is :D

It doesn't have any SFB (0.00%) on e200 and with remarkably low SFS as well.
```
dusk
  x f d p q  j ' o u .
  n s t c y  m h a e i
  b v k g w  z l _ / ,
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

To get rid of `W` inner key (and optimize SFS and SFB), `Dusk_optimized` moved `P` to be with `BN`, and in doing so, it gets rid of the inner corner key and achieves even lower SFB and SFS. However, the cost of it is a whopping 1.41% increase in half scissors according to Keysolve.

I hesitate to recommend `Dusk_optimized` for the following reasons:

- Words like `prob`, `problem`, `public` being 2 row ring jump (much more freq than `f_v` or `f__v` on `Dusk`).

- Frequent `nk` half scissor.

- Worse `ng` and `g_t`.

```
dusk_optimized
  z p d g q  j ' o u .
  s n t c y  m h a e i
  f b k w v  x l _ / ,
        r                   

MONKEYRACER:
  Alt: 29.10%
  Rol: 49.88%   (In/Out: 21.12% | 28.76%)
  One:  1.69%   (In/Out:  0.65% |  1.05%)
  Rtl: 51.57%   (In/Out: 21.77% | 29.81%)
  Red:  3.48%   (Bad:     0.39%)

  SFB: 0.46%
  SFS: 3.81%    (Red/Alt: 1.12% | 2.69%)

  LH/RH: 46.91% | 53.09%
```

## How did you make the figures in [Layout](./layout.md)?
It is from [here](https://keymap-drawer.streamlit.app/) with the following setting:
```
layout:
  qmk_keyboard: chocofi
  #qmk_layout: LAYOUT_split_3x5_2
layers:
  DEF:
    - [X, F, D, P, Q, J, "'", O, U, .]
    - [N, S, T, C, Y, M, H, A, E, I]
    - [B, V, K, G, W, Z, L, "_", /, ","]
    - {}
    - {t: R}
    - {}
    - {}
    - {t: Space}
    - {}

```
