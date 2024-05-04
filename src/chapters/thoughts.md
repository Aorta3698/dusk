# My Thoughts
<!-- toc -->

## 11 Days In
I have been using `Dusk` for 11 days (as of 04/27/2024) and I am currently typing this documentation with it. I am about 60 WPM on MonkeyType E200 tests now and 50 WPM on E10k test (both 2-min tests and with 99% accuracy).

With my current typing speed, I have yet to observe any glaring issues with it. 

I rarely feel any SFB or SFS at all thanks to `Dusk`'s impressive stats, and the major gripe that other people have: `LSB` and `W position` don't bother me at all. 

Additionally, I like the fact that it has almost all the common shortcuts on my left hand: 
`CTRL-C`, `CTRL-V`, `CTRL-X`, `CTRL-W`, `CTRL-D`. The only regrettable thing is `CTRL-Z` and `CTRL-A` being 2 hands.

When it comes to vim, I am editing this documentation with `Helix` and I think it is usable. I got used to using `Canary-ortho` on `Neovim` and `Helix`, and I don't see how `Dusk` is worse than `Canary-ortho` when it comes to vim motion.


But of course, no layout is perfect, despite its impressive stats, `Dusk` isn't without its own problems. The below I list out all criticism that `Dusk` has received and all the minor annoyances I have noticed while using `Dusk`.

## Criticism
Dusk has received some criticism in the first 14 days from the Alt Keyboard Layout community and I've summarized them below (sorted by frequency):
| # of Complaints | Complaint |
|-----------------|-----------|
|       4         | `W` position is subpar for how frequent it is
|       3         | `K` position creates `CK` and `SK` half scissors - deal breaker |
|       2         | `V` position creates `NV` scissors and an awkard `DV` and it is bad |
|       2         | `'` position is questionable
|       2         | `OUL` as in `should` redirection sucks
|       1         | `DV` as in `advice` is somewhat common - deal breaker |

I've attempted to address some complaints by suggesting alternative key placements which are found throughout this documentation, but ultimately `Dusk` is not designed for everyone.

## Awkward Sequences
These are the sequences that I personally find awkward.
All frequency below are obtained from Cmini with SHAI corpus
with the command ```!cmini examples <pattern>```. Only those `>= 0.010%` are documented.

| Pattern | Example    | Classification   | Frequency| 
|---------|------------|------------------|----------|
| `w_p`   | `swap`     | 2.236u SFS       | 0.010%   |
| `p_w`   | `power`    | 2.236u SFS       | 0.059%   |
| `b_x`   | `box`      | 2u Pinky SFS     | 0.026%   |
| `f_v`   | `five`     | 2u Ring SFS      | 0.054%   |
| `k_d`   | `asked`    | 2u Middle SFS    | 0.152%   |
| `p__g`  | `shipping` | 2u Index SFS     | 0.184%   |
| `k__d`  | `kind`     | 2u Middle SFS    | 0.052%   |
| `u,`    | `you,`     | Pinky-ring FSS   | 0.045%   |
| `nv`    | `involve`  | Pinky-ring HSB   | 0.162%   |
| `e.`    | `me.`      | Pinky-ring HSB   | 0.655%   |
| `b_f`   | `before`   | Pinky-ring FSS   | 0.103%   |
| `dv`    | `advice`   | awkward          | 0.075%   |
| `k_p`   | `skip`     | Middle-Index FSS | 0.022%   |
| `dw`    | `hardware` | awkward          | 0.021%   |
| `wd`    | `powder`   | awkward          | 0.011%   | 
| `SUM`   |            | Sum of all above | 1.631%   | 

The long list above seems daunting, but is actually a vast improvement over `Canary-ortho`.

#### Magic Dusk
If you'd like a keyboard layout without any flaw, you should look into magic keyboard layouts in which there exists a magic key that does your custom commands based on surrounding inputs.

It may be possible to make `Dusk` a magic layout, for examples, you can swap `'_` and replace `_` with a magic key on top index (that's where most magic layouts have their magic key).

If you want to learn more about magic layouts, you may want to check out [Ikcelaks's repo](https://github.com/Ikcelaks/keyboard_layouts/blob/main/magic_sturdy/magic_sturdy.md).

## `Dusk` vs. `Canary-ortho`

### Scissors
Info obtained from Keysolve.

| Metric | Diff       | Dusk  | Canary |
|--------|------------|-------|--------|
|  HSB   |  -1.28%    | 2.09% | 3.37%  |
|  HSS   |  -1.65%    | 4.68% | 6.33%  |
|  FSB   |  -0.08%    | 0.02% | 0.10%  |
|  FSS   |  -0.47%    | 0.11% | 0.58%  |

### 2u SFS
Info obtained from Cyanophage.

| Metric    | Diff       | Dusk  | Canary |
|-----------|------------|-------|--------|
|  2u SFS   |  -0.04%    | 0.11% | 0.15%  |

It doesn't take the hidden ones like `v__y`, `b__k`, and `p__k` in `Canary-ortho` into account (`very`, `back`, `park`), so in actuality, it is better than just 0.04% reduction.

### Various info
Info obtained from Oxeylyzer.

| Metric            | Diff         | Dusk       | Canary     |
|-------------------|--------------|------------|------------|
|  SFB              |  -0.347%     | 0.525%     | 0.869%     |
|  SFS              |  -3.058%     | 4.911%     | 7.969%     |
|  Finger Speed     |  -7.512      | 17.338     | 24.850     |
|  Top Finger Speed |  -4.795      | 2.744 (RP) | 7.539 (LI) |
|  LSB              |  -0.358%     | 2.175%     | 2.533%     |

### Quotes
Info obtained from Cmini with Monkeyracer corpus.

| Metric | Diff       | Dusk   | Canary |
|--------|------------|--------|--------|
|  SFB   |  -0.58%    | 0.38%  | 0.96%  | 
|  SFS   |  -3.87%    | 3.76%  | 7.63%  |
|  Red   |  +0.04%    | 3.33%  | 3.29%  |
|  Alt   |  +4.49%    | 28.16% | 23.67% |
|  Rol   |  +0.86%    | 47.99% | 47.13% |

Note that 28.16% is not considered to be high alt. `Graphite` has 31.94% and `Semimak-JQ` has 32.66%. `Canary-ortho` having 23.67% alt is remarkably low and it was designed to be that way.

### Flowy-meter
This is subjective.

| Metric | Dusk   | Canary  |
|--------|--------|---------|
| Flowy  | No     | Yes     |
| Fun    | Mid    | High    |
| Top    | ?      | 213 WPM |

Canary is a solid layout based on Colemak-DH and is fun to type on (at lower speed). It is gained some recognition in the past few years and can now be found on [Keybr](https://www.keybr.com/layouts). It is not to say that Canary is un-usable at high speed; in fact, there are 5 people who have cleared 200 WPM with Canary as of April 2024. I still do like Canary and can recommend it if you can look past its flaws.




## Addressing `P_W` and `W_P`
I do not think it is worth it to swap `WQ` or `PG` to address this 2.24u SFS. Instead, addressing it by hitting `P` with middle finger and `W` with index finger is my suggestion.

## Closing
Overall, I believe `Dusk` is an improvement over `Canary-ortho` in a lot of ways and I am happy with how it turns out.
