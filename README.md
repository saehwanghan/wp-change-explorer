# Within-Person Change Explorer

An interactive teaching tool for **HDF 380K.3 · Analyzing Development & Change**.
It generalizes the random effects of time across the shapes of within-person change:
set the **shape of the mean trajectory** (linear, quadratic, or piecewise) and the
**random effects** (the G-side) that let people differ from the average curve, then watch
individual trajectories, the total variance over time, and the implied correlation
matrix update together.

**Live page:** https://saehwanghan.github.io/wp-change-explorer/

## What it shows
- **Individual trajectories** — a spaghetti plot of simulated people around the average
  (fixed) curve; the random intercept spreads them vertically, a random slope fans them out.
- **Total variance over time** — Var(y_t) across occasions, showing why repeated measures
  are not equally variable once slopes vary.
- **Implied correlation matrix** — the pattern the random effects induce; add an AR(1)
  residual (rho) to see it contribute little once random effects are in the model
  (the R-side / G-side story).

## The R-side companion
Pairs with the [Covariance Structure Explorer](https://saehwanghan.github.io/covariance-explorer/):
together they show how the random effects (G) and the residual structure (R) each shape
the covariance among repeated measures.

## Run it locally
A single self-contained file — open `index.html` in any modern browser. The only
external dependency is Google Fonts (loaded over the network).

## Editing / redeploying
Edit `index.html` and push to `main`; GitHub Pages redeploys automatically.
