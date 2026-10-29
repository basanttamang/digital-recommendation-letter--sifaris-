# Sifaris Feasibility Study — Explained Simply

*A plain-language walkthrough of the project, for anyone with no technical background.* Oct 28, 2026

---

## The problem, in one sentence

Ward offices issue recommendation letters (sifaris) on paper that need the chairperson's signature — and if the chairperson is away, citizens must return another day, and banks or offices receiving the letter can't easily check it's genuine.

## The question this study answers

**Before anyone builds anything: is it actually worth fixing, and which fix is best?** That's what a feasibility study is for — it comes *before* any building starts.

> Like checking whether a house renovation is worth it at all — and comparing a small fix against a full extension — before any hammer swings.

---

## The story, in 6 steps

### Step 1 — List every realistic option, not just one

Rather than jumping to "build an app," four real options were written down and compared fairly:

| Option | What it means |
| --- | --- |
| 0. Do nothing | Keep today's paper process — the baseline everything else is measured against |
| A. Better paper | Give each letter a serial number and keep a register — cheap, quick, no new technology |
| B. QR-verifiable digital letter | The chairperson signs from a phone or laptop, even remotely; a QR code on the printed letter lets anyone scan and verify it's genuine |
| C. National app integration | Issue letters through Nepal's official Nagarik government app |

> Like comparing several real estate agents before picking one, not just going with the first name you hear.

### Step 2 — Score each option on the same scale

Seven criteria were chosen — does it stop fake letters, does it cut return trips, how much does it cost, does it work without a smartphone, and so on — each given a **weight** (how much it matters), and every option scored 1 (poor) to 5 (good) on each one.

| Criterion | Weight |
| --- | --- |
| Stops fake or altered letters | 20% |
| Fewer return trips when the signer is absent | 20% |
| Cost to build and run | 15% |
| Works for citizens without smartphones | 15% |
| Time to deliver | 10% |
| Technical risk | 10% |
| Staff training needed | 10% |

**Result:** Option B (QR digital) scored highest at **3.75 out of 5** — just ahead of Option A at **3.60**.

> Like comparing phones on a spec sheet instead of picking the shiniest one on a shelf.

### Step 3 — Stress-test the result (the step most people skip)

A close score (3.75 vs 3.60) isn't a sure thing — so the weights were deliberately nudged to see if the winner would change.

| If the weights shift slightly toward cost... | Paper (A) | Digital (B) | Winner |
| --- | --- | --- | --- |
| As originally weighted | 3.60 | **3.75** | B |
| Small shift toward cost | **3.75** | 3.65 | A |
| Larger shift toward cost | **3.90** | 3.55 | A |
| All criteria weighted equally | **4.00** | 3.57 | A |

**What this proved:** the "winner" depends on priorities that aren't fully confirmed yet. That's an honest finding, not a weakness — it's exactly why the recommendation below is cautious.

> Like asking "would I still pick this car if fuel price mattered a bit more to me?" — and discovering the answer changes.

### Step 4 — Recommend the safe path, not the flashy one

Because the result was close and some assumptions were unconfirmed, the recommendation was **phased**, not a big-bang rollout:

1. **Now (month 1):** roll out the cheap paper fix (Option A) everywhere — low risk, immediate benefit
2. **Pilot (months 2–4):** trial the QR digital letter (Option B) in just **one ward**
3. **Decide (month 5):** only roll Option B out to all 32 wards if the pilot actually proves itself against clear success measures

> Like test-driving a car for a weekend before committing to buy the whole fleet.

### Step 5 — Check it's actually legal

Before recommending digital signatures, Nepal's **Electronic Transactions Act, 2063 (2008)** was checked to confirm electronic records and digital signatures are legally recognised — so the idea is not just technically possible, but actually allowed. A few specific questions (can a chairperson delegate signing authority when away?) were flagged as still needing legal confirmation.

### Step 6 — Write down what could go wrong, and the plan for each

| Risk | Response |
| --- | --- |
| Digital signatures not legally accepted for these letters | Get a legal opinion before building anything |
| Receiving offices don't bother scanning the QR code | Involve 3–5 receiving offices directly in the pilot |
| Chairperson doesn't want to sign on a phone | Involve them early in the design; allow a trusted delegate to sign instead |
| Ward internet or power goes down | Letters can be prepared offline and signed once connected; paper stays as a fallback |
| Fake QR codes linking to look-alike sites | Verification only works on the official government domain |

---

## The one-breath answer for an interview

> "Before recommending a digital system, I compared four options with a weighted scoring model, stress-tested the result by varying the weights, found the top choice wasn't certain, and recommended a cheap fix immediately plus a small one-ward pilot before any full rollout — backed by a check of Nepal's electronic transactions law."

---

## Where each step lives in the project files

| Step | Where to find it |
| --- | --- |
| 1–2. Options and scoring | `docs/feasibility-study.md` sections 5–6 · `scoring/options-scoring.csv` |
| 3. Sensitivity check | `docs/feasibility-study.md` section 6 ("How sure is this result?") |
| 4. Recommendation and rollout plan | `docs/feasibility-study.md` sections 1 and 9 |
| 5. Legal check | `docs/feasibility-study.md` section 7 |
| 6. Risks | `docs/feasibility-study.md` section 10 |
