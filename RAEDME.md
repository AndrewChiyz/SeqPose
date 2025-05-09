# SeqPose
**SeqPose: An End-to-End Framework to Unify Single-frame and Video-based RGB Category-Level Pose Estimation.**

## 🔥 Overview
Category-level object pose estimation is a longstanding and fundamental task crucial for augmented reality and robotic manipulation applications. 
Existing RGB-based approaches struggle with multi-stage settings and heavily rely on off-the-shelf techniques, such as object detectors, depth estimators, non-differentiable NOCS shape alignment, etc. 
Extra dependencies lead to the accumulation of errors and complicate the whole pipeline, limiting the deployment of these approaches in practical applications. 
This paper streamlined an end-to-end framework unifying the single-frame and video-based category-level pose estimation. 
Specifically, instead of explicitly introducing extra dependencies, the DINOv2 encoder and depth decoder, as robust semantic and geometric prior extractors, are leveraged to produce intra-frame hierarchical semantic and geometric features. A spatial-temporal sparse query network is developed to model the implicit correspondence and inter-frame correlations between a set of implicit 3D query anchors and intra-frame features. Finally, a pose prediction head is employed using the bipartite matching algorithm. 
Experimental results demonstrate that our model achieves state-of-the-art performance compared with RGB-based categorical pose estimation methods on the REAL275 and CAMERA25 datasets.

<div align="center">
<img src="./assets/overview.png" />
</div>
