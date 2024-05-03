# My Thoughts
<!-- toc -->

## 11 Days In
I have been using `Dusk` for 11 days (as of 04/27/2024) and I am currently typing this documentation with it. I am about 60 WPM on MonkeyType E200 tests now and 50 WPM on E10k test (both 2-min tests and with 99% accuracy).

With my current typing speed, I have yet to observe any glaring issues with it. 

I rarely feel any SFB or SFS at all thanks to `Dusk`'s impressive stats, and the major gripe that other people have: `LSB` and `W position` don't bother me at all. 

Additionally, I like the fact that it has almost all the common shortcuts on my left hand: 
`CTRL-C`, `CTRL-V`, `CTRL-Z`, `CTRL-W`, `CTRL-D`. The only regrettable thing is `CTRL-X` and `CTRL-A` being 2 hands.

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
|       1         | `B` position sucks

I've attempted to address some complaints by suggesting alternative key placements which are found throughout this documentation, but ultimately `Dusk` is not designed for everyone.

## Awkward Sequences
These are the sequences that I personally find awkward.
All frequency below are obtained from Cmini with SHAI corpus
with the command ```!cmini examples <pattern>```. Only those `>= 0.010%` are documented.

| Pattern | Example    | Classification   | Frequency| 
|---------|------------|------------------|----------|
| `w_p`   | `swap`     | 2.236u SFS       | 0.010%   |
| `p_w`   | `power`    | 2.236u SFS       | 0.059%   |
| `k_d`   | `asked`    | 2u Middle SFS    | 0.152%   |
| `f_v`   | `five`     | 2u Ring SFS      | 0.054%   |
| `p__g`  | `shipping` | 2u Index SFS     | 0.184%   |
| `k__d`  | `kind`     | 2u Middle SFS    | 0.052%   |
| `u,`    | `you,`     | awkward          | 0.045%   |
| `bs`    | `jobs`     | Pinky-ring HSB   | 0.109%   |
| `nv`    | `involve`  | Pinky-ring HSB   | 0.162%   |
| `e.`    | `me.`      | Pinky-ring HSB   | 0.655%   |
| `b_v`   | `above`    | Pinky-ring FSS   | 0.029%   |
| `dv`    | `advice`   | awkward          | 0.075%   |
| `k_p`   | `skip`     | Middle-Index FSS | 0.022%   |
| `ox`    | `box`      | awkward          | 0.047%   |
| `dw`    | `hardware` | awkward          | 0.021%   |
| `wd`    | `powder`   | awkward          | 0.011%   | 
| `SUM`   |            | Sum of all above | 1.687%   | 

The long list above seems daunting, but is actually a vast improvement over `Canary-ortho`.

#### Side Notes
If you'd like a keyboard layout without any flaw, you should look into magic keyboard layouts in which there exists a magic key that does your custom commands based on surrounding inputs.

It may be possible to make `Dusk` a magic layout, but I am personally not into magic layouts.

## `Dusk` vs. `Canary-ortho`

### Scissors
Info obtained from Keysolve.

| Metric | Difference | Value (Dusk) |
|--------|------------|-------|
|  HSB   |  -1.27%    | 2.10% |
|  HSS   |  -1.13%    | 5.20% |
|  FSB   |  -0.08%    | 0.02% |
|  FSS   |  -0.45%    | 0.13% |

### 2u SFS
Info obtained from Cyanophage.

| Metric | Difference | Value (Dusk) |
|--------|------------|-------|
|  2u SFS   |  -0.04%    | 0.11% |

It doesn't take the hidden ones like `v__y`, `b__k`, and `p__k` in `Canary-ortho` into account (`very`, `back`, `park`), so in actuality, it is better than just 0.04% reduction.

### Various info
Info obtained from Oxeylyzer.

| Metric | Difference | Value (Dusk) |
|--------|------------|-------|
|  SFB   |  -0.342%    | 0.527% |
|  SFS   |  -3.019%    | 4.950% |
|  Finger Speed   |  -1.882    | 4.189 |
|  Top Finger Speed | -0.877 | 0.769 | 
|  LSB   |  -0.354%    | 2.179% |

### Quotes
Info obtained from Cmini with Monkeyracer corpus.

| Metric | Difference | Value (Dusk) |
|--------|------------|--------|
|  SFB   |  -0.58%    | 0.38%  |
|  SFS   |  -3.86%    | 3.77%  |
|  Red   |  +0.03%    | 3.32%  |
|  Alt   |  +4.55%    | 28.22% |
|  Rol   |  -0.82%    | 47.95% |

Note that 28.22% is not considered to be high alt. `Graphite` has 31.94% and `Semimak-JQ` has 32.66%. `Canary-ortho` having 23.67% alt is remarkably low and it was designed to be that way.

## Addressing `P_W` and `W_P`
I do not think it is worth it to swap `WQ` or `PG` to address this 2.24u SFS. Instead, addressing it by hitting `P` with middle finger and `W` with index finger is my suggestion.

## Closing
Overall, I believe `Dusk` is an improvement over `Canary-ortho` in a lot of ways and I am happy with how it turns out.
