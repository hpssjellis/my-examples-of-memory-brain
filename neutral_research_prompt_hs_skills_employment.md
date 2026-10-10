# Research Prompt: High School Preparation for Skilled Work, 1900–2050

**Paste everything below the line into any LLM. For comparison, run it in several models and compare the CSVs.**

---

You are a research team of an education economist, a labour-market historian, and a forecasting methodologist. Your job is to **estimate and compare**, not to advocate. If the evidence is weak, say so and give wide ranges.

## Question

How well have public high schools in the United States prepared young people for skilled, living-wage work from 1900 to 2020, and what plausible range of outcomes might 2020–2050 hold under AI-driven economic change? Then, as one of several candidate responses, assess whether a hands-on electronics/robotics/mechatronics course could change outcomes, and by how much.

Treat the following as **open claims to test, not facts**. For each, state what the evidence supports, contradicts, or leaves unknown:

- C1. Heavy smartphone/social-media/gaming use reduces sustained attention or learning among teenagers.
- C2. Reduced attention or practical experience lowers employment readiness.
- C3. Project-based, hands-on technical courses improve persistence, problem-solving, or employability.
- C4. AI will reduce entry-level skilled work faster than it creates it.

For every claim, also give the strongest argument **against** it and the best evidence that could falsify it.

## Step 1: Define the outcome

- Pick **one country** (default: United States; use Canada only if you can cite comparable historical data). Do not blend national statistics.
- Define a single outcome and keep it fixed across all decades, e.g. "share of an age-18 cohort in skilled, living-wage work within five years." State what counts as *skilled*, what counts as a *living wage* (use real wages relative to a cost-of-living benchmark), and how you treat further study, self-employment, and military service.
- Distinguish: employment, employability, readiness, underemployment, earnings.
- State plainly how the population changed (e.g. high school graduation rose from a small minority to a large majority) and how that limits cross-era comparison.

## Step 2: Historical series, 1900–2020 (every 10 years)

For each decade give: estimate, lower bound, upper bound, **evidence grade**, and a one-sentence rationale.

Evidence grades: **A** direct measurement of the defined outcome; **B** reliable proxy (e.g. graduation rates, youth unemployment, occupational shares, real wage series); **C** synthesis of several proxies; **D** judgment with little data.

Rules:
- Do not choose a shape in advance. Let the evidence set the level and direction, including flat or declining stretches.
- Ranges are judgment-based unless you can compute a statistical interval; label them accordingly.
- Do not attribute any change to smartphones, social media, or other single causes unless you cite evidence for the specific period, and note correlation versus causation.
- Name the three decades where your estimate is least reliable and why.

## Step 3: The wider learning environment

Treat "6 hours at school, 18 elsewhere" as a rough framework, not a measurement. Review evidence on both benefits and harms of digital media, sleep, work, family, and independent learning. Report effect sizes where they exist, note study quality (randomised, longitudinal, cross-sectional, self-report), and say where the research is contested.

## Step 4: Compare candidate interventions

Evaluate at least these on the **same criteria** (evidence quality, plausible effect on readiness, plausible effect on actual employment, cost per student, teacher preparation burden, equity of access, risk of failure or no effect):

1. Status quo
2. Conventional STEM or CS courses
3. Vocational / career-technical education (CTE)
4. Apprenticeship or work-experience programs
5. Other project-based learning
6. A hands-on electronics/robotics/mechatronics course (microcontrollers, sensors, actuators, programming, debugging, networked devices, AI-assisted development)

Rules:
- Separate **skills gained** from **jobs obtained**. A course can build skills with no jobs available.
- Address **selection bias**: students who choose such courses may already be motivated.
- Report existing evidence on robotics/CTE/project-based outcomes with study type and sample. If good causal evidence is missing, say so.
- Consider that effects could be zero or negative for some students or regions.
- Cover who might benefit most and least (by prior skills, gender, rural/urban, region, post-secondary plans).

## Step 5: Scenarios, 2020–2050 (every 10 years)

Build scenarios with **explicit, adjustable assumptions**:

- **Baseline** (no new intervention): low, central, high AI-displacement cases.
- **Intervention** (robotics course introduced): defined by two parameters you must state: (a) **adoption**, the share of each cohort taking the course, and (b) **per-participant effect**, the change in the outcome for those who take it. The population-level effect is roughly adoption × per-participant effect.
- Use a **range** for each parameter, including **zero effect** as a low case. Do not choose parameters to produce a target gap.
- Run a **sensitivity table** (adoption × effect) and identify which assumption drives the result most.
- Include non-education drivers: AI adoption pace, demand for physical and technical work, inequality, demographics, regional labour markets, availability of further training.
- Treat 2020 as a methodological transition, not an economic break. Only use 2030 as a milestone if you justify it.

## Step 6: Deliverables

1. **CSV** with columns: `Decade, Historical_Estimate_Pct, Historical_Lower, Historical_Upper, Evidence_Grade, Baseline_Pct, Baseline_Lower, Baseline_Upper, Intervention_Pct, Intervention_Lower, Intervention_Upper, Assumptions, Sources`. Use blanks for unavailable values. Future values are scenarios, never observations.
2. **Chart** (or full plotting code) titled "High School Graduates Skills to Employment (1900–2050)". Visually separate evidence grades A–B from C–D, show ranges, and include a second panel showing the intervention-minus-baseline gap. Label it an **illustrative index** unless every value is defensibly the same measured quantity.
3. **Written analysis** covering:
   - What the historical trajectory suggests, and which values are least certain
   - Whether credible evidence exists for C1–C4, with the strongest counter-evidence
   - What assumptions determine the baseline–intervention gap and how sensitive it is
   - Who and where benefits most or least
   - Three low-cost school-based experiments to test the hypothesis (design, outcome measures, comparison group, how to limit selection bias)
   - What evidence is needed before using this as a basis for education policy
4. **Conclusion** in plain language for teachers, parents, employers, and policymakers, including at least one conclusion that would *disappoint* a supporter of the intervention and one that would disappoint a sceptic.

## Integrity rules

- Cite only sources you are confident exist. Mark uncertain citations as "unverified" and do not invent titles, authors, statistics, or URLs.
- Distinguish **observed**, **estimated**, and **assumed** in every table and chart.
- Prefer a wide, honest range over false precision.
- If a result depends mainly on your assumptions rather than evidence, say so directly.
- At the end, list the three findings you are least confident about and what would change your mind.
