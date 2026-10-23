# Agentic Engineering

**Building Secure, Human-Centered SaaS with AI Tools**

A complete practical book in notebook form.

Code generation has become inexpensive. Verification has not. That economic shift is the reason this discipline exists.

This volume treats *agentic engineering* as the practice of specifying, directing, verifying, and operating software when large language models and coding agents perform most of the construction work. The subject is not a vendor. It is a durable loop:

**Specify → Generate → Verify → Refine**

The book is written for engineers and founders who intend to ship a multi-tenant Software-as-a-Service product—not a demonstration. Every chapter binds three constraints together:

1. **AI-native construction** — agents write the majority of the code.
2. **Security protocols** — OWASP, TLS, authentication, authorization, tenancy isolation, and supply-chain hygiene are first-class requirements, not a later audit.
3. **HCI guidelines** — Nielsen’s heuristics, Microsoft’s Human–AI Interaction guidelines, accessibility, and agency over automation.

---

## This is not vibe coding

Vibe coding treats the model as an oracle and the repository as a scratchpad.

Agentic engineering treats the model as a capable but untrusted junior colleague who must work inside a harness: typed contracts, tests the agent can run, architectural rules written as files the agent reads on every session, and a human who remains accountable for what ships.

Accountability does not move to the model. “The agent wrote it” is not a defense.

---

## The loop that does not expire

| Phase | Human work | Agent work | Failure mode if skipped |
|---|---|---|---|
| Specify | Problem, constraints, acceptance tests, threat model | Restate the spec; ask clarifying questions | Building the wrong system quickly |
| Generate | Scope one vertical slice | Edit files, write tests, run commands | Unbounded diffs and architectural drift |
| Verify | Review for security, HCI, and intent | Run lint, unit, integration, and e2e suites | Shipping vulnerabilities and dead ends |
| Refine | Convert defects into rules and evals | Patch under the same spec | Repeating the same class of error |

Tools change. The loop does not.

---

## What you will find

The notebook is the book. Sixteen chapters and an executable appendix:

1. What Agentic Engineering Is
2. The Product You Are Actually Building
3. An Agent-Friendly Technical Stack
4. Specification Before Generation
5. Security Protocols for AI-Assisted SaaS
6. Human–Computer Interaction and Human–AI Guidelines
7. Architecture for Multi-Tenant SaaS
8. The Construction Loop
9. Identity, Sessions, and Authorization
10. Data, Privacy, and Tenancy Isolation
11. Testing, Evaluation, and Stopping Conditions
12. Operations: Observability, Cost, and Incident Response
13. From Prototype to Production
14. Worked Example: A Vertical Slice
15. Ethics, Accountability, and the Inverted Week
16. Master Checklists

**Appendix A — Executable Patterns** encodes the rules as standard-library Python: standing agent rules, RBAC, tenant-scoped stores and negative tests, invitation tokens, session cookies, webhook signatures, rate limits and token budgets, prompt isolation, HCI copy, feature-spec objects, CI policy checks, and a production-readiness score.

---

## Who this is for

- Engineers who will remain accountable after typing ceases to be scarce
- Founders shipping multi-tenant SaaS that accepts money and stores other people’s data
- Teams that want agents inside a harness rather than an unbounded chat window

It is not a tutorial for a particular model, editor, or framework. Popularity of a stack matters because agents perform better on well-represented patterns. Popularity is a quality-of-generation consideration, not a religion.

---

## How to use the notebook

Open [`Agentic_Engineering_Ebook.ipynb`](./Agentic_Engineering_Ebook.ipynb) in Jupyter, VS Code, or Google Colab.

1. Read the one-page product brief requirements before any agent opens a file.
2. Treat `AGENTS.md` (Chapter 3 and Appendix A.1) as a standing prompt, not documentation for humans.
3. Execute the appendix cells. They require only Python 3 and the standard library.
4. Port the patterns into your stack. Keep the negative tests—especially cross-tenant denial.
5. Do not mark a session finished unless the slice specification’s acceptance checks would pass.

The chapters state the method. The cells make the method executable.

---

## Production bar (abbreviated)

A product may charge money when all of the following are true:

- TLS everywhere, HSTS on
- Passwords hashed; sessions hardened; MFA available for privileged users
- Every tenant query is scoped and tested negatively
- Backups restore
- Errors are monitored
- Billing webhooks are verified and idempotent
- Terms, privacy policy, and a human contact exist
- Critical paths have end-to-end coverage in CI
- A user can export or delete their tenant data

Until then you have a prototype, regardless of how polished the interface looks.

---

## Authors

| Author | Affiliation |
|---|---|
| **Rishabh Aryan** <sup>*</sup> | M.Tech (AI and Data Science), IIIT Bhagalpur |
| **Anju** | M.Sc. (Mathematics with Computer Science), Maharishi Dayanand University, Rohtak |
| **Satpal** | M.Sc. (Chemistry), Rayat Bahra University, Mohali |
| **Nishtha Kalia** | BCA, MCM DAV College for Women, Panjab University, Chandigarh |

<sup>*</sup> Corresponding author — [rishabh.250201011@iiitbh.ac.in](mailto:rishabh.250201011@iiitbh.ac.in) · [ORCID 0009-0004-7595-9440](https://orcid.org/0009-0004-7595-9440)

### Guide

**Dr. Sarwan Singh**  
Scientist D and Joint Director, NIELIT Ropar  
[ORCID 0000-0001-7062-2129](https://orcid.org/0000-0001-7062-2129)

---

## Citation

```bibtex
@misc{aryan2026agentic,
  title        = {Agentic Engineering: Building Secure, Human-Centered SaaS with AI Tools},
  author       = {Aryan, Rishabh and Anju and Satpal and Kalia, Nishtha},
  year         = {2026},
  note         = {Practical book in notebook form},
  howpublished = {GitHub repository}
}
```

---

## License

Specify the license before publication. Until then, all rights remain with the authors.

---

Specify what must exist. Generate within a harness. Verify as if the author were untrusted—because the author is a statistical model. Refine the harness so the next hour is safer than the last.

That is the whole method. The tools will change. The method should not.

## 🔗 Other repositories by Rishabh Aryan

| Repository | Description | Live |
|---|---|---|
| [100-days-of-python](https://github.com/Rishabh-bgp/100-days-of-python) | My original, offline, no-API-key solutions to all 100 projects of the 100 Days of Code Python bootcamp curriculum… | — |
| [beed-ml-study](https://github.com/Rishabh-bgp/beed-ml-study) | Provenance audit and leakage-aware benchmark of seizure-type classifiers on the Bangalore EEG Epilepsy Dataset — IIT… | — |
| [boston-house-price-prediction](https://github.com/Rishabh-bgp/boston-house-price-prediction) | Boston house price prediction with machine learning: scikit-learn gradient boosting, repeated K-fold CV, race… | [open](https://rishabh-bgp.github.io/boston-house-price-prediction/) |
| [Brain-Computer-Interfaces-and-Cognitive-Computing-An-Introduction](https://github.com/Rishabh-bgp/Brain-Computer-Interfaces-and-Cognitive-Computing-An-Introduction) | Brain–computer interfaces (BCIs) link neural activity to external devices, translating brain signals via algorithms… | — |
| [building-a-virtual-cell-in-python](https://github.com/Rishabh-bgp/building-a-virtual-cell-in-python) | A cell has a normal gene-activity pattern. Knock out one gene and that pattern changes. This project trains a small… | — |
| [california-house-price-prediction](https://github.com/Rishabh-bgp/california-house-price-prediction) | California house price prediction with machine learning: scikit-learn gradient boosting, repeated K-fold and spatial… | [open](https://rishabh-bgp.github.io/california-house-price-prediction/) |
| [Chronic-Kidney-Disease-Stage-Identification-in-HIV-Infected-Patients-Using-Supervised-ML](https://github.com/Rishabh-bgp/Chronic-Kidney-Disease-Stage-Identification-in-HIV-Infected-Patients-Using-Supervised-ML) | ML is transforming Chronic Kidney Disease (CKD) detection in HIV patients, catching early asymptomatic stages to… | — |
| [cobratate](https://github.com/Rishabh-bgp/cobratate) | Cobratate, an esoteric imperative programming language. Tate-flavored syntax, ordinary semantics, and a Python… | [open](https://rishabh-bgp.github.io/cobratate/) |
| [coda-synth](https://github.com/Rishabh-bgp/coda-synth) | CoDA-Synth: stylometric detection of LLM-rewritten dark-web documents with sparse TF-IDF + LinearSVC. Research lab,… | [open](https://shale-ember-delta-kite.grok.me/) |
| [IIT-ROPAR-GENAI-FOUNDATIONS](https://github.com/Rishabh-bgp/IIT-ROPAR-GENAI-FOUNDATIONS) | Free open-source Generative AI foundations ebooks (2026) covering Claude, Grok, Gemini, Cursor, OpenAI and more —… | — |
| [iris-classification](https://github.com/Rishabh-bgp/iris-classification) | Iris flower classification in Python: scikit-learn model comparison, tuning and evaluation, FastAPI /predict API,… | [open](https://rishabh-bgp.github.io/iris-classification/) |
| [kbc-game](https://github.com/Rishabh-bgp/kbc-game) | Kaun Banega Crorepati (KBC) quiz game for the terminal in Python: 16-question prize ladder, safe levels and 4… | — |
| [knn-classifier](https://github.com/Rishabh-bgp/knn-classifier) | Simple K-Nearest Neighbors classifier on the classic Iris dataset using scikit-learn. Loads data, trains the model,… | — |
| [linear-regression-model-](https://github.com/Rishabh-bgp/linear-regression-model-) | Supervised linear regression on the scikit-learn diabetes dataset. A single feature (BMI) is used to predict… | — |
| [logistic-regression](https://github.com/Rishabh-bgp/logistic-regression) | This graduate capstone applies multi-class logistic regression to the Iris dataset. It includes EDA, stratified… | — |
| [logistics-website-capstone](https://github.com/Rishabh-bgp/logistics-website-capstone) | Logistics website capstone: Kargonaut Logistics, a premium freight site mixing claymorphism, glassmorphism and… | [open](https://rishabh-bgp.github.io/logistics-website-capstone/) |
| [lovelight-leap](https://github.com/Rishabh-bgp/lovelight-leap) | 💖 Lovelight Leap: a love-themed 2D platformer in vanilla JS canvas. 4 worlds, a boss you cheer up, original… | [open](https://rishabh-bgp.github.io/lovelight-leap/) |
| [machine-learning-part-1](https://github.com/Rishabh-bgp/machine-learning-part-1) | Machine learning in Python with scikit-learn: heart disease classification and medical insurance cost regression… | — |
| [Meeting-of-Machines-Consumer-Agents-Seller-Agents-and-Hidden-Fulfilment-Risk-in-Online-Retail](https://github.com/Rishabh-bgp/Meeting-of-Machines-Consumer-Agents-Seller-Agents-and-Hidden-Fulfilment-Risk-in-Online-Retail) | Agentic commerce lets shopping and seller agents place orders without showing operational truth. This IS case argues… | — |
| [morocco-city-aware-load-forecasting](https://github.com/Rishabh-bgp/morocco-city-aware-load-forecasting) | City-aware short-term load forecasting and peak detection on high-resolution Moroccan smart-meter data (5 zones).… | — |
| [NIELIT-DATA-SCIENCE](https://github.com/Rishabh-bgp/NIELIT-DATA-SCIENCE) | Hands-on NumPy, Pandas, and Matplotlib Jupyter notebooks for the NIELIT Data Science curriculum — practical,… | — |
| [NIELIT-MACHINE-LEARNING-PROJECTS](https://github.com/Rishabh-bgp/NIELIT-MACHINE-LEARNING-PROJECTS) | Nineteen end-to-end machine learning projects: classification, regression, clustering, and recommendation, with… | — |
| [NIELIT-PYTHON-](https://github.com/Rishabh-bgp/NIELIT-PYTHON-) | Open-source Python teaching notebooks: a language reference and five capstone programs, with detailed documentation.… | — |
| [pan-cancer-classification](https://github.com/Rishabh-bgp/pan-cancer-classification) | Leakage, equivalence, conformal reliability and data efficiency on the UCI TCGA Pan-Cancer RNA-Seq dataset — IIT… | — |
| [Predicting-Hot-Events-in-the-Early-Period-through-Bayesian-Model-for-Social-Networks](https://github.com/Rishabh-bgp/Predicting-Hot-Events-in-the-Early-Period-through-Bayesian-Model-for-Social-Networks) | This notebook details the implementation and evaluation of a Bayesian perspective Early stage Event Prediction… | — |
| [prediction-as-power](https://github.com/Rishabh-bgp/prediction-as-power) | Laboratory and working paper on prediction as power in European electricity markets. A DE-like hourly simulator… | — |
| [real-estate-valuation-taiwan](https://github.com/Rishabh-bgp/real-estate-valuation-taiwan) | Taiwan real estate valuation (Xindian, New Taipei): house price per ping prediction with scikit-learn gradient… | [open](https://rishabh-bgp.github.io/real-estate-valuation-taiwan/) |
| [snakes-and-ladders](https://github.com/Rishabh-bgp/snakes-and-ladders) | 🐍🪜 Original Snakes & Ladders browser game: hand-drawn SVG snakes and ladders, 3D dice, 2-4 humans or bots, sound,… | [open](https://rishabh-bgp.github.io/snakes-and-ladders/) |
| [spam-scan](https://github.com/Rishabh-bgp/spam-scan) | Explainable spam, phishing & Indian-scam detector for SMS/email (English, Hindi, Hinglish): TF-IDF + Logistic… | [open](https://spam-scan.onrender.com) |
| [vedic-math-hybrid-kt](https://github.com/Rishabh-bgp/vedic-math-hybrid-kt) | Hybrid Vedic Math AI: rule-based sutras (Urdhva-Tiryagbhyam, Nikhilam, Yavadunam) plus RF classifier that cleans… | — |
| [wind-turbine-power-model](https://github.com/Rishabh-bgp/wind-turbine-power-model) | Single-turbine power curves + wind-farm simulation. Weibull wind stats, hourly NASA-style speed data, and… | — |
| [zoo-website-capstone](https://github.com/Rishabh-bgp/zoo-website-capstone) | Capstone project: a fictional zoo website built twice — a beginner-style simple version and a cinematic advanced… | [open](https://rishabh-bgp.github.io/zoo-website-capstone/) |
