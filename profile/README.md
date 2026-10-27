# Termondt Tech

**Automated trading systems that a human can monitor and stop.**

I build the infrastructure behind a systematic trading operation: market data, decision support, automated execution and risk controls, with hard safety rails in place from the first day. Since 2026 I have been building it by guiding AI coding agents, under rules they have to obey and reviews they have to pass. That produced [Argus](https://github.com/Termondt-Tech/argus-platform), a platform that traded a real brokerage account at minimum size and whose first strategy was shut down on pre-registered evidence. The write-up is public, including what went wrong.

---

## 📊 What I build

**Market data and decision support**
Pipelines that take in live market data, score opportunities against a defined strategy, and put ranked, explained decisions in front of a person, with every decision written to an audit log.

**Automated execution and risk controls**
Systems that place, watch and close trades by rule, with the rails that make that safe: one place in the code that can send an order, limits enforced twice, and a kill switch that halts new risk without abandoning the positions it is protecting.

**Monitoring and operational reliability**
A hash-chained audit trail with one enforced writer, reconciliation against the broker before anything resumes, and alerting that fires when something is wrong, including when the thing that is wrong is silence.

---

## 🧠 How I build

The same loop whether the code is written by me or by an AI agent I am directing.

**Specify.** What the system must do and must never do, each "never" with the reason it exists. The rules file is read before any code is touched, every time.
**Build.** Design first, naming the alternatives rejected. Sign-off before implementation. Then code, tests, and a review of the build against the design.
**Prove.** Shadow, then the broker's sandbox, then live at the smallest size allowed. Research is pre-registered: the questions and the stopping rule are committed before the data is seen.
**Operate.** A status page, alerts, and a kill switch reachable from a phone. Every incident becomes a rule, and every rule becomes a mechanism.

---

## 📂 What is public here

- [argus-platform](https://github.com/Termondt-Tech/argus-platform): a reference implementation of the platform, published to be read, not run. The constitution the agent worked under, the decision records, the architecture documents, the source, the test suite and the going-live records. Code under Apache-2.0, documents under CC BY 4.0. The example strategy lost money, and `RESULTS.md` says so.

Argus, July to October 2026, by the numbers: 435 commits in 14 weeks, 3,540 tests, 87 decision records, a 741-line rules file read at the start of every session, and one strategy shut down on the evidence.

Nothing here is investment advice.

---

## 📝 The write-up

- Part one: [I guided an AI to build and run a live trading desk. Here is what it took to make that safe.](https://termondttech.com/blog/guided-ai-trading-desk)
- Part two: [How a strategy earns capital: the research platform behind Argus](https://termondttech.com/blog/argus-research-platform)

---

## ✅ How I operate

- **Automated and watched.** Fully automated systems that a human can monitor and stop, in one action, from a phone.
- **Fourteen years in trading infrastructure.** Order-entry gateways at the New York Stock Exchange; market connectivity, FPGA and DevOps at Chicago Trading Company.
- **Guided AI, under rules.** An AI agent writes the code. It reads a written rules file every session and goes through the same reviews I ran for engineers.
- **Evidence over spin.** The first strategy lost money and was stopped. The write-up says so, with the numbers.

---

## Get in touch

Two ways to work with me: a two-week Rails Review for teams putting AI-written code into production, and trading infrastructure built to run automatically and to be monitored and stopped by a human.

✉️ [Contact me](https://termondttech.com/form/contact)
🔗 [termondttech.com](https://termondttech.com)
