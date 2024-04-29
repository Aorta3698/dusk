# My Thoughts
<!-- toc -->

## 11 Days In
I have been using `Dusk` for 11 days (as of 04/27/2024) and I am currently typing this documetation with it. I am about 60 WPM on MonkeyType E200 tests now and 50 WPM on E10k test (both 2-min tests and with 99% accuracy).

With my current typing speed, I have yet to observe any glaring issues with it. 

I rarely feel any SFB or SFS at all thanks to `Dusk`'s impressive stats, and the major grip that other people have: `LSB` and `W position` don't bother me at all. 

Additionally, I like the fact that it has almost all the common shortcuts on my left hand: 
`CTRL-C`, `CTRL-V`, `CTRL-Z`, `CTRL-W`, `CTRL-D`. The only regrettable thing is `CTRL-X` being 2 hands.

When it comes to vim, I am editing this documentation with `Helix` and I think it is usable. I got used to using `Canary-ortho` on `Neovim` and `Helix`, and I don't see how `Dusk` is worse than `Canary-ortho` when it comes to vim motion.


But of course, no layout is perfect, despite its impressive stats, `Dusk` isn't without its own problems. The below I list out all the minor annoyances I have noticed while using `Dusk`.

## Nickpicking
All frequency below are obtained from Cmini with SHAI corpus
with the command ```!cmini examples <pattern>```. Only those `>= 0.010%` are documented.

The `bad` just means that I do not like them, but they may not have been considered as scissor with the conventional definition.
`BAD` means worse than just `bad`.

| Pattern | Example    | Classification   | Frequency| 
|---------|------------|------------------|----------|
| `w_p`   | `swap`     | 2.236u SFS       | 0.010%   |
| `p_w`   | `power`    | 2.236u SFS       | 0.059%   |
| `k_d`   | `asked`    | 2u Middle SFS    | 0.152%   |
| `f_v`   | `five`     | 2u Ring SFS      | 0.054%   |
| `p__g`  | `shipping` | 2u Index SFS     | 0.184%   |
| `k__d`  | `kind`     | 2u Middle SFS    | 0.052%   |
| `o,`    | `also,`    | Pinky-ring bad   | 0.082%   |
| `nf`    | `info`     | Pinky-ring bad   | 0.193%   |
| `e,`    | `me,`      | Pinky-ring bad   | 0.545%   |
| `ui`    | `quite`    | Pinky-ring bad   | 0.355%   |
| `iu`    | `medium`   | Pinky-ring bad   | 0.021%   |
| `u,`    | `you,`     | Pinky-ring BAD   | 0.045%   |
| `bs`    | `jobs`     | Pinky-ring HSB   | 0.109%   |
| `nv`    | `involve`  | Pinky-ring HSB   | 0.162%   |
| `e.`    | `me.`      | Pinky-ring HSB   | 0.655%   |
| `b_v`   | `above`    | Pinky-ring FSS   | 0.029%   |
| `dv`    | `advice`   | Middle-ring FSB  | 0.075%   |
| `k_p`   | `skip`     | Middle-Index FSS | 0.022%   |
| `ox`    | `box`      | Middle-Index bad | 0.047%   |
| `dw`    | `hardware` | Middle-Index bad | 0.021%   |
| `wd`    | `powder`   | Middle-Index bad | 0.011%   | 
| `SUM`   |            | Sum of all above | 2.883%   | 

The long list above seems daunting, but is actually a vast improvement over `Canary-ortho`.

#### Side Notes
If you'd like a keyboard layout without any flaw, you should look into magic keyboard layouts in which there exists a magic key that does your custom commands based on surrounding inputs.

It may be possible to make `Dusk` a magic layout, but I am personally not into magic layouts.

## `Dusk` vs. `Canary-ortho`

### Scissors (Keysolve):
- 1.27% less HSB at 2.10%
- 1.13% less HSS at 5.20%
- 0.08% less FSB at 0.02%
- 0.45% less FSS at 0.13%

### 2u SFS (Cyanophage):
- 0.04% less 2u SFS at 0.11%

It doesn't take the hidden ones like `v__y`, `b__k`, and `p__k` in `Canary-ortho` into account (`very`, `back`, `park`), so in actuality, it is better than just 0.04% reduction.

### Various info (Oxeylyzer):
- 0.342 less SFB at 0.527%
- 3.019 less SFS at 4.950%
- 1.882 less finger speed at 4.189 
- 0.354 less LSB at 2.179%

### Quotes (Cmini with Monkeyracer corpus):
- 0.58% less SFB at 0.38%
- 3.86% less SFS at 3.77%
- 0.03% more redirection at 3.32%

## Closing
Overall, I believe `Dusk` is an improvement over `Canary-ortho` in a lot of ways and I am happy with how it turns out.
