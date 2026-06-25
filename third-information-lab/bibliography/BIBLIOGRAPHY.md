# Bibliography: *Material and Meaning, and the Third Information Lab*

Verified sources for the position paper's empirical claims. Each row gives the claim, the figure as the source actually states it, the verdict, and a link. Verified 2026-06-25 by independent web-search agents against primary sources, with a second adversarial pass on the financial and forecast claims. Verdict legend is in `README.md`.

## Ecological psychology: body-scaled affordances

These ground the keystone's load-bearing premise, that consequential affordances are non-separable (body-scaled, so they do not factor into a property of the environment times a property of the body).

| Claim | As found | Verdict | Source |
|---|---|---|---|
| Passability is the aperture-to-shoulder-width ratio, critical value near 1.3 | The action boundary is A/S = 1.30 (confirmed). But the paper attributes the *perceptual* scaling variable to **eyeheight**, not shoulder width. Shoulder width defines the boundary; eyeheight is what the visual system reads. | partially-verified | Warren & Whang, "Visual guidance of walking through apertures," *J. Exp. Psychol. HPP* 13(3):371-383, **1987**. DOI [10.1037/0096-1523.13.3.371](https://doi.org/10.1037/0096-1523.13.3.371). PMID 2958586 |
| Stair climbability is body-scaled, riser-to-leg-length ratio critical at ~0.88 | Verified. The climbable/unclimbable boundary is a constant proportion of leg length; critical pi (R/L) = 0.88. | verified | Warren, "Perceiving affordances: visual guidance of stair climbing," *J. Exp. Psychol. HPP* 10(5):683-703, **1984**. DOI [10.1037/0096-1523.10.5.683](https://doi.org/10.1037/0096-1523.10.5.683). PMID 6238127 |
| Reachability is body-scaled (Carello et al. 1989) | Verified. Long-armed vs short-armed differences in perceived max reach vanish when data are body-scaled. Reaching is body-scaled but posture- and layout-dependent, not arm length alone. | verified | Carello, Grosofsky, Reichel, Solomon & Turvey, "Visually perceiving what is reachable," *Ecological Psychology* 1(1):27-54, **1989**. DOI [10.1207/s15326969eco0101_3](https://doi.org/10.1207/s15326969eco0101_3) |

## Clinical AI: scale and validation

| Claim | As found | Verdict | Source |
|---|---|---|---|
| FDA listed >1,250 AI/ML medical devices by mid-2025, up from under 400 in 2020 | ">1,250 by July 2025, up from 950 in August 2024" verified. The "under 400 in 2020" is a defensible inference from cumulative authorization data (the FDA list began in 2022 at ~343), not a published 2020 tally. | partially-verified | Bipartisan Policy Center, "FDA Oversight: Understanding the Regulation of Health AI Tools," **2025**. [bipartisanpolicy.org](https://bipartisanpolicy.org/issue-brief/fda-oversight-understanding-the-regulation-of-health-ai-tools/) |
| Taxonomy of 1,016 authorizations, radiology ~74%, none used LLMs | 1,016 count and "none yet involve LLMs" verified verbatim (data cutoff Sept 27, 2024, not mid-2025). The ~74% radiology figure is FDA-panel-derived; the paper frames image analysis as the most common but declining share. | partially-verified | Singh et al., "How AI is used in FDA-authorized medical devices: a taxonomy across 1,016 authorizations," *npj Digital Medicine*, **2025**. DOI [10.1038/s41746-025-01800-1](https://doi.org/10.1038/s41746-025-01800-1). PMID 40596700 |
| External validation is scarce relative to published models; a barrier to safe adoption | Verified. Only 10 of 59 orthopedic-outcome ML models were externally validated; broader reviews concur development-only studies dominate. | verified | Groot et al., "Availability and reporting quality of external validations of machine-learning prediction models," *Acta Orthopaedica*, **2021**. DOI [10.1080/17453674.2021.1910448](https://doi.org/10.1080/17453674.2021.1910448) |

## The collapse cases

| Claim | As found | Verdict | Source |
|---|---|---|---|
| Epic Sepsis Model externally validated, 145,885 encounters, sensitivity 14.7%, PPV 7.6% | Verified to the decimal. Two county EDs (Harris Health, Houston), calendar-year 2023 data, published 2024. | verified | Ostermayer et al., "External validation of the Epic sepsis predictive model in 2 county emergency departments," *JAMIA Open*, **2024**. DOI [10.1093/jamiaopen/ooae133](https://doi.org/10.1093/jamiaopen/ooae133). PMC11560849 |
| Earlier validation: missed 67% of sepsis, alerted on 18% of hospitalized patients | Verified exactly. 1,709 of 2,552 sepsis patients missed (67%); alerts on 6,971 of 38,455 (18%); AUC 0.63 vs developer's claimed 0.76-0.83. | verified | Wong et al., "External Validation of a Widely Implemented Proprietary Sepsis Prediction Model," *JAMA Internal Medicine* 181(8):1065-1070, **2021**. DOI [10.1001/jamainternmed.2021.2626](https://doi.org/10.1001/jamainternmed.2021.2626) |
| Cost-as-proxy algorithm on ~200M/year; correction raises Black share flagged from 17.7% to 46.5% | Verified exactly. "Remedying this disparity would increase the percentage of Black patients receiving additional help from 17.7 to 46.5%." ~200M/year is the paper's industry estimate of the tool class's reach (widely identified as Optum Impact Pro). | verified | Obermeyer, Powers, Vogeli, Mullainathan, "Dissecting racial bias in an algorithm used to manage the health of populations," *Science* 366(6464):447-453, **2019**. DOI [10.1126/science.aax2342](https://doi.org/10.1126/science.aax2342). PMID 31649194 |

## EHR burden

| Claim | As found | Verdict | Source |
|---|---|---|---|
| PCPs spend 5.9h of an 11.4h day in the EHR, with after-hours documentation | 5.9h of 11.4h verified verbatim. After-hours EHR time is **1.4 hours (86 min)**, not the 2.7h the draft originally stated (corrected). | verified | Arndt et al., "Tethered to the EHR," *Annals of Family Medicine* 15(5):419-426, **2017**. DOI [10.1370/afm.2121](https://doi.org/10.1370/afm.2121). PMC5593724 |
| Clinicians override 49-96% of safety alerts | Verified. 49-96% is the classic overall override range. | verified | van der Sijs et al., "Overriding of Drug Safety Alerts in CPOE," *J. Am. Med. Inform. Assoc.* 13(2):138-147, **2006**. DOI [10.1197/jamia.M1809](https://doi.org/10.1197/jamia.M1809). PMC1447540 |
| 88.2% of very-severe drug-drug-interaction alerts overridden | Verified verbatim. 33,888 of 38,409 very-severe DDI alerts overridden (acceptance 11.8%). | verified | Van De Sijpe et al., "Overall performance of a drug-drug interaction clinical decision support system," *BMC Med. Inform. Decis. Mak.* 22:48, **2022**. DOI [10.1186/s12911-022-01783-z](https://doi.org/10.1186/s12911-022-01783-z). PMC8864797 |
| Each additional documentation hour, ~7.1% fewer outside records viewed | Verified exactly. Associational (not causal); documentation burden "crowds out" health information exchange use. | verified | Holmgren, Adler-Milstein, Apathy, "Electronic Health Record Documentation Burden Crowds Out Health Information Exchange Use," *Health Affairs* 43(11):1538-1545, **2024**. DOI [10.1377/hlthaff.2024.00398](https://doi.org/10.1377/hlthaff.2024.00398) |

## The engineering of attention

| Claim | As found | Verdict | Source |
|---|---|---|---|
| A wealth of information creates a poverty of attention | Verified verbatim. | verified | Herbert A. Simon, "Designing Organizations for an Information-Rich World," in M. Greenberger (ed.), *Computers, Communications, and the Public Interest*, Johns Hopkins University Press, **1971**, pp. 40-41 |
| Engagement-maximizing recommenders have a structural incentive to manipulate; long-horizon RL shifts preferences | Verified. "Systems trained via long-horizon optimization will have direct incentives to manipulate users." (Mechanism is preference-shift; "beliefs" is a slight extension.) | verified | Carroll, Dragan, Russell, Hadfield-Menell, "Estimating and Penalizing Induced Preference Shifts in Recommender Systems," *ICML 2022*, PMLR 162:2686-2708. arXiv [2204.11966](https://arxiv.org/abs/2204.11966) |
| 2025 OpenAI/MIT 4-week RCT: heavy chatbot use correlated with loneliness, dependence, less socializing | Verified, with nuance: the loneliness/dependence/reduced-socializing results are **correlations with voluntary usage intensity**; the randomized arms produced no significant effects. The draft says "correlated with," which is precise. | partially-verified | Fang, Liu et al. (MIT Media Lab & OpenAI), "How AI and Human Behaviors Shape Psychosocial Effects of Chatbot Use," arXiv [2503.17473](https://arxiv.org/abs/2503.17473), **2025** |

## The attention economy and the ad duopoly

| Claim | As found | Verdict | Source |
|---|---|---|---|
| Behavioral surplus and surveillance capitalism | Verified verbatim against the book's definitions ("free raw material," "behavioral surplus," "prediction products"). | verified | Shoshana Zuboff, *The Age of Surveillance Capitalism*, PublicAffairs, **2019**. ISBN 978-1-61039-569-4 |
| Meta forecast to overtake Google in worldwide digital ad revenue in 2026 | Forecast, single outlet. eMarketer (Dec 2025) projects Meta $243.46B vs Google $239.54B in 2026. 2025 actuals still favor Google. Attributed as forecast. | projection-or-forecast | EMARKETER, "Meta to Surpass Google in Digital Ad Revenues for First Time Ever," **2025**. [emarketer.com](https://www.emarketer.com/learningcenter/guides/meta-to-surpass-google-in-digital-ad-revenues-for-first-time-ever/) |
| Google ~$214B, Meta ~$196B ad revenue in 2025 | These are eMarketer **net worldwide digital ad revenue** estimates, NOT company-reported. Alphabet's SEC-reported FY2025 Google ad revenue was ~$294.7B. The draft now labels the metric. | partially-verified | EMARKETER (estimate); Alphabet Inc. FY2025 8-K (reported), via [CNBC, Feb 4 2026](https://www.cnbc.com/2026/02/04/alphabet-googl-q4-2025-earnings.html) |

## Frontier-lab economics

| Claim | As found | Verdict | Source |
|---|---|---|---|
| OpenAI: $122B committed at $852B valuation; ~$13.1B 2025 revenue; ~$34B costs | Verified. Round closed March 31, 2026. 2025 revenue $13.07B, costs $34B (audited financials, FT-verified). | verified | OpenAI, "OpenAI raises $122 billion," **2026** ([openai.com](https://openai.com/index/accelerating-the-next-phase-ai/)); costs via [Where's Your Ed At / FT](https://www.wheresyoured.at/exclusive-openai-financials/) |
| OpenAI targeting ~$600B compute spend by 2030 | A forward investor **target**, revised down from an earlier ~$1.4T figure. Not committed or realized spend. | projection-or-forecast | [CNBC, Feb 20 2026](https://www.cnbc.com/2026/02/20/openai-resets-spend-expectations-targets-around-600-billion-by-2030.html) |
| Anthropic: $65B at $965B valuation, run-rate revenue crossing ~$47B | Verified verbatim against Anthropic's own announcement. $47B is run-rate (annualized), not trailing realized revenue. | verified | Anthropic, "Anthropic raises $65B in Series H," **2026**. [anthropic.com/news/series-h](https://www.anthropic.com/news/series-h) |
| OpenAI ChatGPT ads Jan 2026 / free tiers Feb; ~$1B 2026 to ~$25B 2029; Google Gemini ads 2026 | Announcement (Jan 16) and Free/Go-tier go-live (Feb 9) verified. The $1B-to-$25B is internal-document "free-user monetization" (ads **plus affiliate**), not pure ad revenue. Google "signaled/explored" Gemini ads but **publicly denied** a firm 2026 rollout. | partially-verified | OpenAI ([blog](https://openai.com/index/our-approach-to-advertising-and-expanding-access/)); [Axios](https://www.axios.com/2026/02/09/chatgpt-ads-testing-go-free); The Information (via reporting); Adweek / [Search Engine Land](https://searchengineland.com/google-corrects-report-claiming-ads-are-coming-to-gemini-in-2026-465856) |

## The wellness and safety landscape

| Claim | As found | Verdict | Source |
|---|---|---|---|
| Google's Search Inside Yourself (2007) pitched on career and business benefits | Verified. Launched 2007 (book 2012); explicit work-performance and EI business framing. | verified | Chade-Meng Tan, *Search Inside Yourself*, HarperOne, **2012**; SIYLI; Knowledge@Wharton |
| Center for Humane Technology led by Silicon Valley insiders | Verified. Co-founded by Tristan Harris (former Google Design Ethicist), Aza Raskin, Randima Fernando. | verified | [humanetech.com/who-we-are](https://www.humanetech.com/who-we-are) |
| McMindfulness: individualized mindfulness deflects structural responsibility; AI-companion engagement-vs-wellbeing tension | Both verified. Purser argues corporate mindfulness shifts responsibility "from society to the individual." A 2026 IJHCI study documents AI-companion sycophancy boosting engagement while harming wellbeing. | verified | Ronald Purser, *McMindfulness*, Repeater Books, **2019**; IJHCI, DOI [10.1080/10447318.2026.2626809](https://doi.org/10.1080/10447318.2026.2626809) |
| Safetywashing: many safety benchmarks correlate with capability | Verified. Benchmarks like TruthfulQA, GPQA, MT-Bench, Chatbot Arena are largely explained by a capabilities component. | verified | Ren et al., "Safetywashing: Do AI Safety Benchmarks Actually Measure Safety Progress?" *NeurIPS 2024*. arXiv [2407.21792](https://arxiv.org/abs/2407.21792) |
| Anthropic Sonnet 4.5: mechanistic analysis to identify and suppress evaluation-awareness | "Identify" verified. "Suppress" was an interpretability **experiment** (a probe to test whether eval-awareness inflated apparent alignment), not a shipped fix; the production mitigation landed with a later model (Opus 4.5). | partially-verified | Anthropic, "System Card: Claude Sonnet 4.5," **2025**. [anthropic.com](https://www.anthropic.com/claude-sonnet-4-5-system-card) |
| Open Philanthropy: ~$336M to AI safety since 2017; 2025 RFP ~$40M / 21 areas | RFP ($40M / 21 areas) verified and official. The $336M is a **third-party community estimate** (McAleese), not an Open Phil figure. Open Phil has rebranded as Coefficient Giving. | partially-verified | Open Philanthropy RFP, **2025** ([EA Forum](https://forum.effectivealtruism.org/posts/XtgDaunRKtCPzyCWg/open-philanthropy-technical-ai-safety-rfp-usd40m-available)); $336M via McAleese, "An Overview of the AI Safety Funding Situation," LessWrong, 2025 |

## Biographical claims (self-reported, on file)

| Claim | As found | Verdict | Source |
|---|---|---|---|
| MPH; clinical-systems and evaluation background | MPH, University of Washington (2025). Change Management Readiness Lead on a Workday ERP integration at Seattle Children's Hospital. Associate Director of Evaluation and Learning for a 60+ partner Health Equity Zone (One Neighborhood Builders). | self-reported, on file | Isaac Rubinstein, resume 2026. The draft's earlier "RIDOH data-modernization track" was corrected to these held credentials; RIDOH was a funder of the Health Equity Zone evaluation work, not a held role. |

## Corrections applied to the position paper

The fact-check changed these in the draft before publication:

1. **EHR after-hours time: 2.7 hours to 1.4 hours.** The 2.7h figure was not in Arndt et al. 2017, which reports 1.4h (86 min); it was conflated from another study.
2. **Google / Meta 2025 ad revenue labeled as eMarketer net-digital estimates,** not company-reported, since Alphabet's reported Google ad revenue (~$294.7B) is far higher than the $214B digital estimate.
3. **OpenAI $600B compute and the Meta-overtakes-Google line attributed as forecasts/targets,** not facts.
4. **OpenAI ad projection reframed** as "free-user monetization" (ads plus affiliate), and the **Google Gemini-ads claim softened** to "signaled while publicly denying a firm 2026 rollout."
5. **FDA "under 400 in 2020" softened** to an inference; the ~74% radiology figure attributed to FDA-panel data.
6. **Anthropic Sonnet 4.5 "suppress" qualified** as an interpretability experiment, not a deployed fix.
7. **Open Philanthropy $336M attributed** as a third-party estimate.
8. **Personal credentials corrected:** "RIDOH data-modernization track" replaced with the actual held roles (MPH UW, Seattle Children's Workday change management, the Health Equity Zone evaluation work).

No claim was refuted outright. The corrections were figures, attributions, and metric mismatches, the failure modes the fact-check exists to catch.
