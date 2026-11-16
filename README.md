<h1 align="center">MHFlow: Multi-Hypothesis Iterative Refinement for Warping-Alone Optical Flow Estimation</h1>

<p align="center">Yingda Huang · Dong Li</p>

<p align="center"><strong>Code coming soon</strong></p>

## Introduction

Warping-alone optical flow estimation uses the current flow estimate to warp high-resolution target features and predict flow updates without constructing cost volumes. However, when this estimate is inaccurate, relying on a single warped target feature map may limit the accuracy of subsequent flow updates. We propose MHFlow, an optical flow framework equipped with a Multi-Hypothesis Iterative Refinement (MHIR) mechanism comprising two modules: the Multi-Hypothesis Warping and Aggregation (MHWA) module and the Dynamic Gated Injection (DGI) module.

<p align="center">
  <a href="mhflow-overview.webp">
    <img src="mhflow-overview.webp" width="90%" alt="MHFlow architecture showing feature extraction and the multi-hypothesis refinement loop">
  </a>
</p>

**Contributions:**

- We propose MHFlow, an optical flow framework equipped with MHIR. The MHWA module aggregates warped features and motion update proposals from multiple local correspondence hypotheses to improve recurrent flow updates.
- We design the DGI module to control feature and motion injection, and introduce hypothesis-aware supervision to train the aggregation weights and motion update proposals.
- We demonstrate competitive performance on Sintel and leading results on KITTI 2015 among the compared two-frame methods, together with strong cross-dataset generalization. Controlled ablations and regional analysis validate the effectiveness of the proposed refinement mechanism.
