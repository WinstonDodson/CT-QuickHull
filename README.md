#CT-QuickHull
Optimal convex hulls for low-rank data in high-dimensional space.
A 35-year-old algorithmic lemma (Clarkson-Shor 1989) turns out to be
conditional independence on a DAG. For data with intrinsic rank r ≪ d,
CT-QuickHull computes the exact convex hull in O(nrd) — matching the
unconditional lower bound Ω(nrd).
Read the essay
The scope-honest essay summarizing the contribution is hosted via GitHub Pages:
Optimal Convex Hulls for Low-Rank Data in High-Dimensional Space
Citation
Dodson, W. (2026). CT-QuickHull: Causal Sparsity on Ancestry DAGs for
Exact Convex Hull Construction (v1.5.1). Zenodo.
DOI: 10.5281/zenodo.20100509
What's in this repository

paper/ — The published preprint as a PDF.
code/ — Reproducibility notebook (ct_quickhull_experiments.ipynb).
Verifies all five theoretical predictions in under five seconds in
Google Colab.
slides/ — Conference deck (10 slides) with the same scope-honest
framing as the paper.
docs/ — The essay HTML, served via GitHub Pages.

Quick start with the notebook
bashgit clone https://github.com/winstondodson/CT-QuickHull.git
cd CT-QuickHull
jupyter notebook code/ct_quickhull_experiments.ipynb
Or open the notebook directly in Google Colab
by uploading code/ct_quickhull_experiments.ipynb. Runs in under 5 seconds.
The contribution by scope
Universal (holds for any data): The Heritage Lemma reframed as
d-separation on an event DAG. The Conflict Tree is a graphical model;
each update is one message-passing step.
Scoped (requires rank r ≪ d): CT-QuickHull achieves O(nrd),
matching the unconditional lower bound Ω(nrd). Three Carathéodory bounds
collapse the output-sensitive formula. Mass pruning at the final step.
Conjectural (open problems): Theorem 0 (the CSS complexity formula)
in full generality. Conjectured CSS instances: Delaunay triangulation,
hyperplane arrangements, sparse matrix refactorization.
§9.1 of the paper is explicit about what is not claimed: for full-rank
or adversarial geometry, the asymptotic order matches existing methods.
Contact
Winston Dodson · Independent Researcher
ORCID: 0009-0001-7148-0764
Email: winstonsdodson@icloud.com
License
Released under Creative Commons Attribution 4.0 International (CC BY 4.0).
Comments, critique, and collaboration on the conjectured CSS instances welcome.