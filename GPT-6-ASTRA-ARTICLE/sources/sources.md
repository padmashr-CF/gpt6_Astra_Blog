# GPT-6 Astra Article — Verified Sources

## Tier 1: Official OpenAI Documentation

1. **OpenAI GPT-6 Astra Announcement**
   - Publisher: OpenAI
   - Date: September 3, 2026
   - URL: https://openai.com/index/gpt-6-astra/
   - Status: Primary source for model capabilities, specifications, and all launch benchmark charts

2. **OpenAI GPT-6 Astra System Card**
   - Publisher: OpenAI (Deployment Safety Hub)
   - Date: September 3, 2026
   - URL: https://deploymentsafety.openai.com/gpt-6-astra
   - Status: Primary source for safety evaluation, alignment findings, CoT monitorability, cybersecurity assessment
   - Note: this is the canonical system card URL. Earlier drafts of this article cited `openai.com/index/gpt-6-astra-system-card/`, which does not appear in any search index — corrected.

3. **Safety overview: GPT-6 Astra**
   - Publisher: OpenAI
   - Date: September 2026
   - URL: https://openai.com/index/safety-overview-gpt-6-astra/
   - Status: Source for development safeguards, Critical designation, Daybreak access restrictions

4. **OpenAI Preparedness Framework**
   - Publisher: OpenAI
   - Date: Updated September 2026
   - URL: https://openai.com/preparedness/
   - Status: Framework under which Astra received "Critical" cybersecurity designation

5. **OpenAI API Documentation — GPT-6 Astra**
   - Publisher: OpenAI
   - URL: https://platform.openai.com/docs/models
   - Status: 1.05M context window, 128K max output, pricing tiers

## Tier 2: Independent Evaluation (third-party measurement)

6. **ARC Prize Foundation — "OpenAI's GPT-6 Astra on ARC-AGI-3"**
   - URL: https://arcprize.org/blog/astra
   - Results: Standard harness (max) **62.7%** at $26,098; OpenAI provider adapter (high) **99.9%** at $18,817
   - Key finding: the difference is state handling, not tools or compute. The Standard harness is provider-neutral and requires the model to carry state forward as *visible notes*; OpenAI's adapter preserves *opaque reasoning state* with compaction. The adapter run was 3.66× faster on 49% fewer tokens.
   - ARC Prize's own caveat: "saturating the benchmark would not represent proof of achieving AGI"
   - Status: **The single most valuable independent datapoint of launch week.**

7. **Artificial Analysis — Intelligence Index & benchmarking**
   - URL: https://artificialanalysis.ai/articles/benchmarking-gpt-6-astra
   - Results: v4.1.1 — Fable 5.1 65.7, Astra 61.2, Sol 60.9. Index revised twice within two days; under v4.3, Astra and Fable 5.1 **tied at 53**, Anthropic holding three of the top four positions.
   - Also: Artificial Analysis's own Terminal-Bench 4.0 run gives Astra (max) 59.1% vs Fable 5.1 52.0% — a different gap from OpenAI's 57.9/55.8.
   - Note: Artificial Analysis (artificialanalysis.ai) is a distinct organization from Emergent (emergent.sh). Earlier drafts conflated them — corrected.

8. **AutomationBench-AA**
   - Publisher: Artificial Analysis, in partnership with Zapier
   - URL: https://artificialanalysis.ai/evaluations/automationbench-aa
   - Status: Independent leaderboard run on Zapier's private benchmark subset

9. **Terminal-Bench public leaderboard**
   - Results: Astra (Codex, max) 58.18%; Fable 5.1 (Claude Code, max) 57.88%; Opus 5 51.82%; Sol 37.27%; Gemini 3.8 Flash (mini-SWE-agent, high) 19.09%
   - Status: Third-party leaderboard; puts the Astra/Fable gap at 0.3 points rather than OpenAI's 2.1

## Tier 3: Benchmark Owners

10. **AutomationBench** — Zapier
    - URL: https://zapier.com/benchmarks · https://github.com/zapier/AutomationBench · arXiv:2604.18934
    - Design: 47 real tools across Sales, Marketing, Operations, Support, Finance, HR. Deterministic final-state assertions, no LLM-as-judge. **Drives simulated REST APIs, not screenshots** — it is not a computer-use benchmark.

11. **FrontierMath / Terminal-Bench / OSWorld / ScreenSpot-Pro / HealthBench** — respective benchmark projects; Astra's scores on these reach the public only via OpenAI's launch charts.

## Tier 4: Major Technology Publications

12. **CSO Online / Computerworld — Sam Altman rollout apology**
    - URL: https://www.csoonline.com/article/4219249/sam-altman-calls-gpt-6-astra-rollout-messy-as-enterprise-users-wait-for-access.html
    - Date: September 4, 2026
    - Verified: "First, sorry for the messy rollout"; Daybreak-only launch-day access; Daybreak Blue for advanced cyber capabilities

13. **Unite.AI — Critical cyber rating**
    - URL: https://www.unite.ai/openai-releases-gpt-6-astra-its-first-model-rated-critical-for-cyber/

14. **Fox Business / Slashdot / TechTimes — Greg Brockman AGI remarks**
    - Verified quotes: "Welcome to the AGI era"; "I think it's not unreasonable to feel that we are now in the AGI era"; "I do leave it up to the reader to decide for themselves if this qualifies for them"

15. **IBTimes UK — official benchmark comparison table**
    - URL: https://www.ibtimes.co.uk/gpt-6-astra-benchmarks-revealed-how-openai-says-it-compares-claude-gpt-56-1817871
    - Status: Renders OpenAI's launch charts including competitor columns

16. **Vellum, DataCamp, OfficeChai, MindStudio** — secondary benchmark write-ups used for cross-checking. Note: these render OpenAI's Terminal-Bench 4.0 figure as **57.7%** where IBTimes and AtlasCloud render it as **57.9%**. The discrepancy is unresolved and is disclosed in the article.

17. **Wikipedia — GPT-6 Astra**
    - URL: https://en.wikipedia.org/wiki/GPT-6_Astra
    - Source for: "recurrent depth" (looped transformer) architecture; >100,000 GPU pretraining run at Stargate Texas (VP Aidan Clark); Jakub Pachocki on safety as a bottleneck

## Tier 5: Social Media & Firsthand Demonstrations

18. **Sam Altman — X, launch post**
    - URL: https://x.com/sama/status/2095600005772104059
    - Date: September 3, 2026, ~7:49 PM
    - Verified verbatim: "GPT-6 Astra is here. We hope it will begin to enable a new generation of entrepreneurship, scientific discovery, and building. We believe it is the best model in the world for computer use, professional work, science, coding, cybersecurity, and more."

19. **Sam Altman — X, rollout apology**
    - Date: September 4, 2026
    - Verified: "First, sorry for the messy rollout."

20. **Sharif Shameem — "I'm Not a Robot" demonstration**
    - URL: https://x.com/sharifshameem/status/2096847916837314853
    - Date: September 7, 2026
    - Verified: "Astra has successfully beat all 48 levels of the 'I'm Not a Robot' game"
    - **Affiliation disclosure: Sharif Shameem works on OpenAI's Labs team (sharif.io).** This is a capability showcase from inside OpenAI, not an independent test. The game is Neal Agarwal's CAPTCHA *parody* on neal.fun, not a production bot-detection system.
