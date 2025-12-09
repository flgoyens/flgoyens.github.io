---
permalink: /research/
title: "Research Projects"
author_profile: true
redirect_from:
  - /md/
  - /research.html
---

<style>
.research-grid {
  display: flex;
  flex-direction: column;
  gap: 2.2rem;
  margin-top: 1rem;
}
.research-card {
  display: grid;
  grid-template-columns: 180px 1fr;
  gap: 1.6rem;
  padding: 1.25rem 1.5rem;
  border: 1px solid #e5e7eb;
  border-radius: 14px;
  background: linear-gradient(135deg, #fbfcff 0%, #f4f7fb 100%);
  box-shadow: 0 18px 40px rgba(15, 23, 42, 0.06);
}
.research-thumb {
  align-self: center;
  display: flex;
  justify-content: center;
}
.research-thumb img {
  width: 100%;
  max-width: 180px;
  border-radius: 10px;
  border: 1px solid #e5e7eb;
  background: #fff;
}
.research-tag {
  display: inline-block;
  font-size: 0.78rem;
  letter-spacing: 0.06em;
  text-transform: uppercase;
  color: #475569;
  margin-bottom: 0.35rem;
}
.research-content h2 {
  margin-top: 0;
  margin-bottom: 0.4rem;
}
.research-blurb {
  margin-bottom: 0.9rem;
  line-height: 1.65;
}
.research-links {
  display: flex;
  flex-wrap: wrap;
  gap: 0.6rem;
}
.research-link {
  display: inline-flex;
  align-items: center;
  gap: 0.35rem;
  padding: 0.45rem 0.75rem;
  border-radius: 8px;
  border: 1px solid #0f172a;
  color: #0f172a;
  font-weight: 600;
  text-decoration: none;
  background: #e0e7ff;
}
.research-link.secondary {
  background: #fff;
  border-color: #cbd5e1;
  color: #1f2937;
}
@media (max-width: 720px) {
  .research-card {
    grid-template-columns: 1fr;
  }
  .research-thumb {
    order: 1;
  }
  .research-content {
    order: 2;
  }
}
</style>

<div class="research-grid">
  <article class="research-card">
    <figure class="research-thumb">
      <img src="/images/image_matrix_recovery.png" alt="Illustration for nonlinear matrix recovery">
    </figure>
    <div class="research-content">
      <span class="research-tag">Optimization on manifolds</span>
      <h2>Nonlinear matrix recovery</h2>
      <p class="research-blurb">
        Reconstruct structured matrices from a small set of affine measurements by enforcing that columns satisfy a nonlinear geometric structure (clusters, algebraic varieties). We cast the problem as a optimization on a smooth manifold and solve it with Riemannian trust-region or alternating minimization.
      </p>
      <div class="research-links">
        <a class="research-link" href="https://arxiv.org/abs/2109.06095">Paper</a>
        <a class="research-link secondary" href="https://github.com/flgoyens/nonlinear-matrix-recovery">Code</a>
      </div>
    </div>
  </article>

  <article class="research-card">
    <figure class="research-thumb">
      <img src="/images/registration_image.png" alt="Illustration for point cloud registration on varieties">
    </figure>
    <div class="research-content">
      <span class="research-tag">Geometric data alignment</span>
      <h2>Point cloud registration on algebraic varieties</h2>
      <p class="research-blurb">
        Align two point clouds of the same object that is well approximated by an algebraic variety. We first estimate the algebraic variety that best approximates the data. Then, we compute the transformation by enforcing that the surfaces of both objects overlap. This handles noisy samples and preserves the shape of the data.
      </p>
      <div class="research-links">
        <a class="research-link" href="https://arxiv.org/abs/2401.08562">Preprint</a>
        <a class="research-link secondary" href="https://github.com/flgoyens/variety-registration">Code</a>
        <!-- <a class="research-link secondary" href="http://flgoyens.github.io/files/dphil_thesis.pdf">Thesis chapter</a> -->
      </div>
    </div>
  </article>

  <article class="research-card">
    <figure class="research-thumb">
      <img src="/images/image_strict_saddle.png" alt="Illustration for strict saddle optimization">
    </figure>
    <div class="research-content">
      <span class="research-tag">Second-order optimization</span>
      <h2>Strict saddle optimization</h2>
      <p class="research-blurb">
        Some nonconvex problems have a strict saddle geometry: strong convexity near minimizers and negative curvature at saddles. We study Riemannian trust-region methods in this setting, showing that they find approximate minimizers with an iteration count that scales only logarithmically with accuracy. We also design an inexact variant that chooses steps using the strict saddle structure, improving complexity guarantees over the general nonconvex case.
      </p>
      <div class="research-links">
        <a class="research-link" href="https://doi.org/10.1007/s10107-024-02156-2">Journal paper</a>
        <a class="research-link secondary" href="https://arxiv.org/abs/2402.07614">Preprint</a>
      </div>
    </div>
  </article>
</div>
