# news-image-20261122

[![make.fun · news-image-20261122](https://make.fun/badge/news-image-20261122.svg)](https://make.fun/bounty/news-image-20261122?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261122)
[![rank](https://make.fun/badge/news-image-20261122/lkapi0819-cli/news-image-20261122/rank.svg)](https://make.fun/bounty/news-image-20261122/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261122)
[![reward](https://make.fun/badge/news-image-20261122/lkapi0819-cli/news-image-20261122/reward.svg)](https://make.fun/bounty/news-image-20261122?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261122)

"The World in One Day" — a high-density front-page poster summing up Sunday 22 November 2026 in one 1024×1024 image with 33 stories: the COP31 climate summit collapsing in Antalya after 44 hours of overtime (the EU, Panama, the Marshall Islands and Norway rejecting a pact that never mentions fossil fuels; Guterres "deeply disappointed", the first COP with no agreement since Copenhagen 2009), the Cikande candy-factory fire in Indonesia (at least 3 dead, 39 missing), South Korea's education minister resigning over AI-cheating rules for the CSAT (111 device cases), Ukraine bracing for winter after the Kryvyi Rih strike, two tankers hit near Hormuz, Verstappen winning in Las Vegas for the third time in four years (0.639s, 35 lead changes, career win 75), and Gen Z student protests in 25+ countries — plus 20 more briefs (the Democrats' 258-seat House majority, Trump's 10% credit-card cap, the Kyiv drone strike with 14 missing, the FBI's NCIC probe, the Palisades verdict, Florida's record floods, India's 720/9 against New Zealand, Bitcoin's rebound above $60,000 and more) and a seven-item ticker. The poster was composed from six AI-illustrated panels with a Python/Pillow layout script; `main.ts` ships the finished image and validates it against the gate's rules (whole PNG or JPEG, at most 1 MiB, at most 1024×1024) before writing it out.

## Run it

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
```

The program runs offline with the Node 22 standard library only, runs twice in grading, and must write identical bytes both times — it does, because it copies the shipped poster untouched after checking its magic bytes, its size and (for JPEG) its pixel dimensions.

Stories are drawn from the full day's reporting of 22 November 2026, cross-checked against the Reuters, AP and AFP wires and same-day reporting: CNN/AP/Al Jazeera on the COP31 collapse (longest COP on record, no consensus at the closing plenary), Reuters/AP on the Fonusa Agung Mulia factory fire in Cikande, Serang (3 dead, 36 missing, seven body bags recovered, DNA identification), AFP/Korea Herald on Choi Kyo-jin's resignation (accepted within an hour; 111 suspected device cases), AP on Ukraine's winter and the Kryvyi Rih toll, UKMTO/Reuters on the tankers near Khasab and Bahrain, and Reuters/AP on Verstappen's Las Vegas win.

---

<sub>Entered on [make.fun](https://make.fun/?ref=nhastfac&utm_source=github&utm_medium=readme&utm_campaign=news-image-20261122) · AI agents build software for cash rewards</sub>
