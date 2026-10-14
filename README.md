# Naive Bayes Lab

An interactive study guide for §9.3–9.4 of Kevin P. Murphy, *Probabilistic Machine Learning: An Introduction*
(naive Bayes classifiers; generative vs discriminative classifiers).

**Live:** https://isaackrallison.github.io/naive-bayes/

Every section has an **Explain it** box at four levels (Kid, High school, Undergrad, Grad / MLE), switchable globally from the top bar.

- **9.3 The naive Bayes assumption:** a six-word spam filter. Toggle words and watch each class's prior × factors, the posterior, and a log-odds "ledger" of votes.
- **9.3.1 Example models:** Bernoulli NB on 7×9 mini-digits (θ pictures like Figure 9.6, a drawing pad, per-pixel "why" map, sample predictions like Figure 9.7, removable classes); categorical NB on fruit; Gaussian NB in 2-D with axis-aligned ellipses vs full-covariance QDA as the true correlation grows.
- **9.3.2 Model fitting:** an editable 12-email training table with live counts, MLEs, and zero-count warnings. It drives the spam filter above.
- **9.3.3 Bayesian naive Bayes:** a pseudo-count slider (MLE → Jeffreys → Laplace → heavy), Beta posteriors, and the 0/0 trap at β̆ = 0.
- **9.3.4 NB and logistic regression:** NB's implied weights, checked against σ(w·x + w₀), and a 1-D Gaussian panel where the log-odds is linear only when σ₁ = σ₂.
- **9.4–9.4.1 Generative vs discriminative:** Figure 9.8 with adjustable wiggle, NB vs logistic regression learning curves (Ng & Jordan crossover), and a duplicated-feature calibration demo.
- **9.4.2 Advantages of generative classifiers:** a scenario sorter and a side-by-side table.
- **9.4.3 Missing features:** tri-state spam words (marginalize vs fill with "absent") and digit occlusion with accuracy over 500 test images.
- Step-by-step math for Eqs. 9.46–9.65, a 40-question quiz tagged by level, and a cheat sheet.

Single self-contained `index.html`, no build step. Loads Google Fonts and MathJax from cdnjs. All data are synthetic and generated in the page from fixed seeds.
