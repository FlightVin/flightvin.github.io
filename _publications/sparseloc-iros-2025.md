---
title: "SparseLoc: Sparse Open-Set Landmark-based Global Localization for Autonomous Navigation"
collection: publications
category: conferences
permalink: /publication/sparseloc-iros-2025
excerpt: 'This paper presents SparseLoc, a global localization system that uses vision-language models to build sparse, semantic maps. It achieves localization accuracy comparable to dense LiDAR methods while using 500x fewer points. Deployed in production by [Ati Motors](https://atimotors.com/)'
date: 2025-03-02
venue: 'IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS)'
paperurl: 'https://arxiv.org/pdf/2503.23465'
# citation: 'Paul, P., Bhat, V., Salian, T., Omama, M., Jatavallabhula, K. M., Arulselvan, N., & Krishna, M. (2025). "SparseLoc: Sparse Open-Set Landmark-based Global Localization for Autonomous Navigation." <i>IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS), 2025</i>.'
---

**SparseLoc** is a novel framework for global localization (finding a robot's position on a map without GPS) that addresses the high storage costs of traditional navigation methods. It does this by creating sparse, semantically-rich maps instead of dense point clouds. Most modern techniques rely on dense LiDAR maps, which are precise but become prohibitively large (often gigabytes) and computationally expensive to scale for city-wide navigation. Other sparse-map approaches often lack the robustness needed for reliable localization.

Our method uses vision-language foundation models (VLMs) in a zero-shot way to identify and map only the *centroids* of static, open-set landmarks (like 'traffic pole' or 'hedge'). This creates a "semantic-topometric" map that is **1/500th the size** of a traditional dense map. For localization, we use a robust Monte Carlo particle filter enhanced with a novel **late optimization** strategy to refine the pose estimate. SparseLoc achieves accuracy comparable to dense-map methods (below 5m and 2° error on KITTI) and dramatically outperforms other sparse-map techniques. It also demonstrates high robustness in challenging cross-dataset localization scenarios. 

Deployed in production by [Ati Motors](https://atimotors.com/) for their industrial navigation usecase. 

More information is available on the [project page](https://reachpranjal.com/sparseloc).
