---
title: "Consistency Checks for Language Model Forecasters"
collection: publications
category: conferences
permalink: /publication/consistency-forecasters
excerpt: 'This paper proposes a new framework for evaluating LLM-based forecasters by measuring their logical consistency, introducing an "arbitrage metric" that correlates strongly with future forecasting accuracy, even when the ground truth is unknown.'
date: 2025-04-23
venue: 'International Conference on Learning Representations (ICLR)'
paperurl: 'https://arxiv.org/pdf/2412.18544'
# citation: 'Paleka, D., Shen, A., Sudhir, A. P., Wang, E., Alvarez, A., Bhat, V., & Tramèr, F. (2025). "Consistency Checks for Language Model Forecasters." <i>International Conference on Learning Representations (ICLR), 2025</i>.'
---

This paper tackles the challenge of evaluating LLM forecasters, especially for long-range predictions where the ground truth is years away. We propose evaluating them not on *accuracy* (which we can't know) but on their *logical consistency*. While recent work shows LLMs are approaching human-level forecasting, evaluating them is a key bottleneck. Prior work on consistency was often limited to simple checks using ad-hoc metrics that are difficult to compare or aggregate.

We introduce a principled new consistency metric based on **arbitrage**: if a forecaster is illogical (e.g., says two mutually exclusive events are both 60% likely), an arbitrageur could make a guaranteed profit. We develop an automated pipeline to generate tuples of logically-related questions (covering negation, conditional probability, etc.) and measure this "arbitrage violation". We show that our instantaneous consistency scores **strongly correlate with the forecaster's true future accuracy** (Brier score). We also introduce `ArbitrageForecaster`, a method to improve consistency, and release a long-horizon benchmark with questions that resolve in 2028.

Additional information could be found in this [Twitter thread](https://x.com/dpaleka/status/1877717539763237346).
