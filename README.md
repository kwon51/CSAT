# CSAT Economics Model Performance Report

Static snapshot of an interactive analysis comparing how different LLMs (GPT, Claude, Gemini, Grok, Solar, EXAONE, ...) perform on Korean CSAT (수능) economics exam questions: accuracy, cost, response speed, and error breakdowns.

## 1. Model Leaderboard

![Composite index by model](images/leaderboard.png)

| Rank | Model | Composite Index | Overall Pass@1 (%) | Valid-Response Pass@1 (%) | Error Rate (%) | Cost (USD) | Avg Response Time (s) |
|---|---|---|---|---|---|---|---|
| 1 | GPT-5.3 Codex (high) | 100.000 | 100.000 | 100.000 | 0.000 | 5.264 | 15.401 |
| 2 | Gemini 3.1 Pro (default) | 99.667 | 99.667 | 99.667 | 0.000 | 7.962 | 15.157 |
| 3 | Gemini 3.1 Pro (xhigh) | 99.333 | 99.333 | 99.333 | 0.000 | 8.087 | 15.986 |
| 4 | Grok-4 (default) | 87.147 | 92.667 | 98.932 | 6.333 | 15.848 | 72.315 |
| 5 | Grok-4 (max) | 86.207 | 91.667 | 97.865 | 6.333 | 15.727 | 68.906 |
| 6 | GPT-5.3 Codex (default) | 54.333 | 54.333 | 54.333 | 0.000 | 0.508 | 1.437 |
| 7 | Claude Sonnet 4.5 (default) | 53.333 | 53.333 | 53.333 | 0.000 | 1.223 | 2.297 |
| 8 | Claude Sonnet 4.5 (max) | 52.333 | 52.333 | 52.333 | 0.000 | 1.236 | 2.183 |
| 9 | K-Exaone 236B (default) | 49.875 | 66.333 | 99.005 | 33.000 | 0.796 | 115.772 |
| 10 | Solar Pro3 (default) | 40.667 | 40.667 | 40.667 | 0.000 | 0.159 | 5.343 |

## 2. Score Performance By Points

### Model by point-value heatmap: Overall Pass@1 (%)

![Model by point-value heatmap: Overall Pass@1 (%)](images/points_overall.png)

### Model by point-value heatmap: Valid-Response Pass@1 (%)

![Model by point-value heatmap: Valid-Response Pass@1 (%)](images/points_valid.png)

## 3. Score Performance By Image Presence

### Model by image-presence heatmap: Overall Pass@1 (%)

![Model by image-presence heatmap: Overall Pass@1 (%)](images/image_presence_overall.png)

### Model by image-presence heatmap: Valid-Response Pass@1 (%)

![Model by image-presence heatmap: Valid-Response Pass@1 (%)](images/image_presence_valid.png)

## 4. Point Value x Image Presence

### Model by point-image segment heatmap: Overall Pass@1 (%)

![Model by point-image segment heatmap: Overall Pass@1 (%)](images/point_image_overall.png)

### Model by point-image segment heatmap: Valid-Response Pass@1 (%)

![Model by point-image segment heatmap: Valid-Response Pass@1 (%)](images/point_image_valid.png)

## 5. Cost And Speed

![Total cost vs average response time](images/cost_speed.png)

## 6. Error Analysis

### API error count by model (cases)

![API error count by model](images/error_count.png)

## 7. Additional Analysis By Difficulty

### Model by difficulty heatmap: Overall Pass@1 (%)

![Model by difficulty heatmap](images/difficulty.png)

## 8. Problem-Level Correctness Views

### Model accuracy by exam type: Overall Pass@1 (%)

![Model accuracy by exam type: Overall Pass@1 (%)](images/exam_type.png)

### 2 pt / No Image: Overall Pass@1 (%)

![2 pt / No Image: Overall Pass@1 (%)](images/segment_2pt_noimage.png)

### 2 pt / Image: Overall Pass@1 (%)

![2 pt / Image: Overall Pass@1 (%)](images/segment_2pt_image.png)

### 3 pt / No Image: Overall Pass@1 (%)

![3 pt / No Image: Overall Pass@1 (%)](images/segment_3pt_noimage.png)

### 3 pt / Image: Overall Pass@1 (%)

![3 pt / Image: Overall Pass@1 (%)](images/segment_3pt_image.png)

### Model accuracy by category: Overall Pass@1 (%)

![Model accuracy by category: Overall Pass@1 (%)](images/category.png)

### Raw correctness grids (per exam)

O = Correct, X = Wrong, ERR = Error/missing. Columns are problem number (see hover text in the original report for point value / image presence per problem).

<details>
<summary>CSAT 2026</summary>

| Model | Q01 | Q02 | Q03 | Q04 | Q05 | Q06 | Q07 | Q08 | Q09 | Q10 | Q11 | Q12 | Q13 | Q14 | Q15 | Q16 | Q17 | Q18 | Q19 | Q20 |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| GPT-5.3 Codex (high) | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O |
| Gemini 3.1 Pro (default) | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O |
| Gemini 3.1 Pro (xhigh) | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O |
| Grok-4 (default) | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O |
| Grok-4 (max) | O | O | O | O | O | O | O | O | O | O | O | O | X | O | O | O | O | O | O | O |
| GPT-5.3 Codex (default) | X | O | X | X | O | X | O | O | X | X | X | O | X | O | X | O | O | O | X | X |
| Claude Sonnet 4.5 (default) | X | O | O | X | O | X | X | O | X | X | X | O | O | O | O | O | X | X | X | X |
| Claude Sonnet 4.5 (max) | X | O | O | X | O | X | O | O | X | X | X | X | X | O | O | O | X | O | X | X |
| K-Exaone 236B (default) | O | O | O | ERR | ERR | ERR | ERR | O | ERR | ERR | O | O | X | O | O | O | O | O | O | X |
| Solar Pro3 (default) | O | O | X | X | X | X | O | O | O | X | X | O | X | X | O | X | O | X | O | X |
</details>

<details>
<summary>CSAT 2025</summary>

| Model | Q01 | Q02 | Q03 | Q04 | Q05 | Q06 | Q07 | Q08 | Q09 | Q10 | Q11 | Q12 | Q13 | Q14 | Q15 | Q16 | Q17 | Q18 | Q19 | Q20 |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| GPT-5.3 Codex (high) | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O |
| Gemini 3.1 Pro (default) | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O |
| Gemini 3.1 Pro (xhigh) | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O |
| Grok-4 (default) | O | O | O | O | O | O | O | O | O | ERR | ERR | O | O | O | O | O | O | O | ERR | O |
| Grok-4 (max) | O | O | O | O | O | O | O | ERR | O | O | ERR | O | O | O | O | O | O | O | O | O |
| GPT-5.3 Codex (default) | O | O | X | O | X | O | X | X | O | X | X | X | X | X | X | O | X | X | X | X |
| Claude Sonnet 4.5 (default) | O | O | X | O | X | O | X | X | O | X | X | O | O | X | X | O | X | X | X | X |
| Claude Sonnet 4.5 (max) | O | O | X | O | X | O | X | X | O | X | X | O | X | X | O | O | X | X | X | X |
| K-Exaone 236B (default) | O | O | O | O | ERR | O | O | ERR | O | ERR | ERR | O | O | ERR | ERR | O | O | ERR | ERR | ERR |
| Solar Pro3 (default) | X | O | X | X | X | O | X | X | O | X | X | O | O | X | X | O | X | X | X | X |
</details>

<details>
<summary>CSAT 2024</summary>

| Model | Q01 | Q02 | Q03 | Q04 | Q05 | Q06 | Q07 | Q08 | Q09 | Q10 | Q11 | Q12 | Q13 | Q14 | Q15 | Q16 | Q17 | Q18 | Q19 | Q20 |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| GPT-5.3 Codex (high) | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O |
| Gemini 3.1 Pro (default) | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O |
| Gemini 3.1 Pro (xhigh) | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O |
| Grok-4 (default) | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O |
| Grok-4 (max) | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O |
| GPT-5.3 Codex (default) | X | O | O | O | X | O | X | O | O | O | X | X | O | X | X | X | X | O | X | X |
| Claude Sonnet 4.5 (default) | X | O | O | X | X | O | X | X | X | X | X | O | O | X | O | X | X | O | X | X |
| Claude Sonnet 4.5 (max) | X | O | O | X | X | O | X | X | X | X | X | O | O | X | O | X | X | O | X | X |
| K-Exaone 236B (default) | ERR | O | O | O | ERR | ERR | O | ERR | ERR | ERR | O | O | O | O | O | O | ERR | O | ERR | ERR |
| Solar Pro3 (default) | X | O | O | X | X | X | X | O | X | X | X | O | X | X | X | O | X | O | X | X |
</details>

<details>
<summary>CSAT 2023</summary>

| Model | Q01 | Q02 | Q03 | Q04 | Q05 | Q06 | Q07 | Q08 | Q09 | Q10 | Q11 | Q12 | Q13 | Q14 | Q15 | Q16 | Q17 | Q18 | Q19 | Q20 |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| GPT-5.3 Codex (high) | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O |
| Gemini 3.1 Pro (default) | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O |
| Gemini 3.1 Pro (xhigh) | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O |
| Grok-4 (default) | O | O | O | O | O | ERR | O | O | O | O | O | O | O | O | O | O | O | O | O | O |
| Grok-4 (max) | O | O | O | ERR | O | O | O | O | O | O | O | O | O | O | ERR | O | O | O | O | O |
| GPT-5.3 Codex (default) | O | O | O | O | O | X | X | X | X | X | O | X | O | X | X | X | O | O | X | X |
| Claude Sonnet 4.5 (default) | X | O | O | X | O | X | X | O | X | O | X | X | O | X | O | X | O | O | X | X |
| Claude Sonnet 4.5 (max) | X | O | X | X | O | O | X | O | X | X | X | X | O | O | O | X | O | O | X | X |
| K-Exaone 236B (default) | ERR | O | O | O | O | ERR | ERR | O | O | ERR | ERR | ERR | O | ERR | ERR | O | O | O | ERR | ERR |
| Solar Pro3 (default) | O | O | X | O | X | O | X | O | X | X | X | X | X | O | X | O | O | X | O | O |
</details>

<details>
<summary>CSAT 2022</summary>

| Model | Q01 | Q02 | Q03 | Q04 | Q05 | Q06 | Q07 | Q08 | Q09 | Q10 | Q11 | Q12 | Q13 | Q14 | Q15 | Q16 | Q17 | Q18 | Q19 | Q20 |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| GPT-5.3 Codex (high) | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O |
| Gemini 3.1 Pro (default) | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O |
| Gemini 3.1 Pro (xhigh) | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O |
| Grok-4 (default) | O | O | O | O | O | O | O | O | O | O | O | ERR | O | O | O | O | O | O | O | O |
| Grok-4 (max) | O | O | O | O | O | O | O | O | O | O | O | ERR | O | O | O | O | O | O | O | ERR |
| GPT-5.3 Codex (default) | O | O | O | O | O | X | O | X | O | X | O | X | O | X | O | O | O | X | X | X |
| Claude Sonnet 4.5 (default) | O | X | O | O | O | X | O | O | O | O | X | X | O | X | O | O | X | O | X | X |
| Claude Sonnet 4.5 (max) | O | X | O | O | O | X | O | O | O | O | O | X | O | X | O | O | X | X | X | X |
| K-Exaone 236B (default) | O | O | O | O | O | ERR | O | O | ERR | ERR | ERR | ERR | O | O | ERR | O | O | O | O | ERR |
| Solar Pro3 (default) | O | O | O | O | X | X | O | X | X | X | X | X | X | X | O | X | X | X | O | O |
</details>

<details>
<summary>MCSAT6 2026</summary>

| Model | Q01 | Q02 | Q03 | Q04 | Q05 | Q06 | Q07 | Q08 | Q09 | Q10 | Q11 | Q12 | Q13 | Q14 | Q15 | Q16 | Q17 | Q18 | Q19 | Q20 |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| GPT-5.3 Codex (high) | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O |
| Gemini 3.1 Pro (default) | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O |
| Gemini 3.1 Pro (xhigh) | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O |
| Grok-4 (default) | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O |
| Grok-4 (max) | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O |
| GPT-5.3 Codex (default) | O | O | O | O | O | X | O | O | X | X | O | X | X | X | O | O | X | X | X | X |
| Claude Sonnet 4.5 (default) | O | O | O | X | O | X | O | O | X | X | O | O | X | O | X | O | X | X | X | O |
| Claude Sonnet 4.5 (max) | O | O | O | X | O | X | O | O | X | X | O | O | X | O | X | O | X | O | X | O |
| K-Exaone 236B (default) | O | O | O | O | O | O | O | ERR | O | O | O | O | O | O | O | O | O | ERR | ERR | O |
| Solar Pro3 (default) | O | O | O | X | X | X | O | O | X | O | X | X | X | X | X | X | X | X | O | O |
</details>

<details>
<summary>MCSAT6 2025</summary>

| Model | Q01 | Q02 | Q03 | Q04 | Q05 | Q06 | Q07 | Q08 | Q09 | Q10 | Q11 | Q12 | Q13 | Q14 | Q15 | Q16 | Q17 | Q18 | Q19 | Q20 |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| GPT-5.3 Codex (high) | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O |
| Gemini 3.1 Pro (default) | X | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O |
| Gemini 3.1 Pro (xhigh) | X | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O |
| Grok-4 (default) | ERR | O | O | O | O | O | O | O | O | O | O | O | O | O | ERR | O | O | O | O | O |
| Grok-4 (max) | ERR | O | O | O | O | O | O | O | O | O | O | O | O | O | ERR | O | O | O | O | O |
| GPT-5.3 Codex (default) | X | O | O | O | X | O | O | X | O | X | O | O | O | O | O | O | O | O | O | X |
| Claude Sonnet 4.5 (default) | X | O | O | O | X | O | O | X | O | O | O | O | O | X | O | O | X | X | O | O |
| Claude Sonnet 4.5 (max) | X | O | O | O | X | O | O | X | O | O | X | O | X | X | X | O | X | X | O | X |
| K-Exaone 236B (default) | ERR | O | O | O | O | O | O | O | O | ERR | O | O | O | O | ERR | O | O | O | O | ERR |
| Solar Pro3 (default) | X | O | X | O | O | O | O | X | X | O | X | O | X | O | X | X | X | X | O | X |
</details>

<details>
<summary>MCSAT6 2024</summary>

| Model | Q01 | Q02 | Q03 | Q04 | Q05 | Q06 | Q07 | Q08 | Q09 | Q10 | Q11 | Q12 | Q13 | Q14 | Q15 | Q16 | Q17 | Q18 | Q19 | Q20 |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| GPT-5.3 Codex (high) | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O |
| Gemini 3.1 Pro (default) | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O |
| Gemini 3.1 Pro (xhigh) | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O |
| Grok-4 (default) | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | ERR | O | O | O | O |
| Grok-4 (max) | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | ERR | O | O | O | O |
| GPT-5.3 Codex (default) | O | O | O | O | X | O | X | O | O | X | X | O | O | O | O | X | O | O | X | O |
| Claude Sonnet 4.5 (default) | X | O | O | O | O | O | O | O | X | X | O | O | O | X | O | X | X | O | O | X |
| Claude Sonnet 4.5 (max) | X | O | O | O | O | O | X | O | X | X | O | O | O | O | O | X | X | O | O | X |
| K-Exaone 236B (default) | ERR | O | O | O | ERR | O | O | O | O | ERR | O | O | O | O | ERR | O | O | O | O | O |
| Solar Pro3 (default) | X | O | O | O | X | O | X | O | X | X | O | O | O | O | X | X | X | X | O | O |
</details>

<details>
<summary>MCSAT6 2023</summary>

| Model | Q01 | Q02 | Q03 | Q04 | Q05 | Q06 | Q07 | Q08 | Q09 | Q10 | Q11 | Q12 | Q13 | Q14 | Q15 | Q16 | Q17 | Q18 | Q19 | Q20 |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| GPT-5.3 Codex (high) | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O |
| Gemini 3.1 Pro (default) | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O |
| Gemini 3.1 Pro (xhigh) | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O |
| Grok-4 (default) | O | O | O | O | O | ERR | O | O | O | O | O | O | O | O | O | O | O | O | O | O |
| Grok-4 (max) | O | O | O | O | O | ERR | O | ERR | O | O | O | O | O | O | O | O | O | O | O | O |
| GPT-5.3 Codex (default) | O | O | O | X | O | X | X | O | O | X | O | O | O | X | X | O | O | X | X | X |
| Claude Sonnet 4.5 (default) | O | O | O | X | O | X | O | O | O | X | O | O | O | X | X | X | O | X | X | X |
| Claude Sonnet 4.5 (max) | O | O | O | X | O | X | O | O | O | X | O | X | O | X | X | X | O | X | X | X |
| K-Exaone 236B (default) | O | O | O | O | O | ERR | ERR | ERR | O | O | O | O | O | O | O | O | O | O | O | ERR |
| Solar Pro3 (default) | O | O | X | O | X | X | O | X | O | X | O | X | O | X | X | X | X | X | X | X |
</details>

<details>
<summary>MCSAT6 2022</summary>

| Model | Q01 | Q02 | Q03 | Q04 | Q05 | Q06 | Q07 | Q08 | Q09 | Q10 | Q11 | Q12 | Q13 | Q14 | Q15 | Q16 | Q17 | Q18 | Q19 | Q20 |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| GPT-5.3 Codex (high) | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O |
| Gemini 3.1 Pro (default) | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O |
| Gemini 3.1 Pro (xhigh) | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O |
| Grok-4 (default) | O | O | O | O | O | O | O | O | O | O | O | O | X | O | O | ERR | O | O | O | ERR |
| Grok-4 (max) | O | O | O | O | O | O | O | O | O | O | O | O | X | O | ERR | X | O | X | O | ERR |
| GPT-5.3 Codex (default) | O | O | O | O | O | O | X | X | X | O | O | O | X | O | X | X | O | X | O | O |
| Claude Sonnet 4.5 (default) | O | O | O | O | O | O | O | X | X | O | O | O | O | O | X | X | O | X | X | O |
| Claude Sonnet 4.5 (max) | O | O | O | O | O | O | O | X | X | O | O | O | X | O | X | X | O | X | X | O |
| K-Exaone 236B (default) | O | O | O | O | O | O | O | O | O | O | O | O | O | O | ERR | ERR | O | O | O | ERR |
| Solar Pro3 (default) | O | O | O | O | O | O | X | X | X | O | X | O | X | X | X | X | X | X | O | X |
</details>

<details>
<summary>MCSAT9 2026</summary>

| Model | Q01 | Q02 | Q03 | Q04 | Q05 | Q06 | Q07 | Q08 | Q09 | Q10 | Q11 | Q12 | Q13 | Q14 | Q15 | Q16 | Q17 | Q18 | Q19 | Q20 |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| GPT-5.3 Codex (high) | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O |
| Gemini 3.1 Pro (default) | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O |
| Gemini 3.1 Pro (xhigh) | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O |
| Grok-4 (default) | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O |
| Grok-4 (max) | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O |
| GPT-5.3 Codex (default) | X | O | X | X | O | O | O | O | O | X | O | X | X | X | X | O | X | X | X | X |
| Claude Sonnet 4.5 (default) | X | O | O | O | O | O | O | O | X | X | O | X | X | X | X | X | X | O | X | X |
| Claude Sonnet 4.5 (max) | O | O | O | O | O | O | O | O | X | O | O | X | X | X | X | X | X | X | O | X |
| K-Exaone 236B (default) | O | O | ERR | ERR | O | ERR | O | O | ERR | O | O | O | O | O | ERR | O | ERR | ERR | ERR | ERR |
| Solar Pro3 (default) | X | X | O | O | O | X | O | X | X | X | X | X | O | X | O | O | X | X | X | X |
</details>

<details>
<summary>MCSAT9 2025</summary>

| Model | Q01 | Q02 | Q03 | Q04 | Q05 | Q06 | Q07 | Q08 | Q09 | Q10 | Q11 | Q12 | Q13 | Q14 | Q15 | Q16 | Q17 | Q18 | Q19 | Q20 |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| GPT-5.3 Codex (high) | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O |
| Gemini 3.1 Pro (default) | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O |
| Gemini 3.1 Pro (xhigh) | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O |
| Grok-4 (default) | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | ERR | O | O | O | O |
| Grok-4 (max) | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | ERR | O | O | O | O |
| GPT-5.3 Codex (default) | O | O | O | X | X | O | X | O | O | X | O | O | X | X | O | X | X | O | X | X |
| Claude Sonnet 4.5 (default) | O | O | O | X | X | O | X | O | O | O | O | X | O | X | O | X | X | O | O | O |
| Claude Sonnet 4.5 (max) | O | O | O | X | X | O | X | O | O | O | O | O | O | X | O | X | X | O | O | X |
| K-Exaone 236B (default) | O | O | O | O | ERR | O | ERR | O | O | ERR | O | O | ERR | ERR | O | ERR | ERR | O | O | ERR |
| Solar Pro3 (default) | O | O | X | O | O | O | X | O | X | X | O | X | X | O | X | X | O | X | X | X |
</details>

<details>
<summary>MCSAT9 2024</summary>

| Model | Q01 | Q02 | Q03 | Q04 | Q05 | Q06 | Q07 | Q08 | Q09 | Q10 | Q11 | Q12 | Q13 | Q14 | Q15 | Q16 | Q17 | Q18 | Q19 | Q20 |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| GPT-5.3 Codex (high) | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O |
| Gemini 3.1 Pro (default) | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O |
| Gemini 3.1 Pro (xhigh) | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O |
| Grok-4 (default) | O | O | O | X | O | O | O | O | ERR | ERR | O | ERR | O | O | O | O | O | O | O | O |
| Grok-4 (max) | O | O | O | X | O | O | O | O | ERR | ERR | O | ERR | O | O | O | O | O | O | O | O |
| GPT-5.3 Codex (default) | X | O | O | O | X | O | O | X | X | X | X | O | O | X | X | X | O | O | O | O |
| Claude Sonnet 4.5 (default) | X | O | O | X | O | X | O | X | X | X | X | O | X | X | X | X | X | O | O | X |
| Claude Sonnet 4.5 (max) | X | O | O | O | O | X | X | X | X | X | X | O | X | X | X | X | X | O | O | X |
| K-Exaone 236B (default) | O | O | O | ERR | O | O | O | O | O | ERR | O | ERR | O | O | ERR | ERR | ERR | O | O | ERR |
| Solar Pro3 (default) | X | O | O | X | X | X | X | X | X | O | O | X | O | X | O | X | O | O | X | X |
</details>

<details>
<summary>MCSAT9 2023</summary>

| Model | Q01 | Q02 | Q03 | Q04 | Q05 | Q06 | Q07 | Q08 | Q09 | Q10 | Q11 | Q12 | Q13 | Q14 | Q15 | Q16 | Q17 | Q18 | Q19 | Q20 |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| GPT-5.3 Codex (high) | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O |
| Gemini 3.1 Pro (default) | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O |
| Gemini 3.1 Pro (xhigh) | O | O | O | O | O | O | O | O | O | O | O | X | O | O | O | O | O | O | O | O |
| Grok-4 (default) | O | ERR | O | O | ERR | O | ERR | O | O | O | O | X | O | O | O | O | O | O | O | O |
| Grok-4 (max) | O | ERR | O | O | O | O | O | O | O | O | O | X | O | O | O | O | O | O | O | O |
| GPT-5.3 Codex (default) | O | X | O | O | O | O | O | X | O | X | X | X | O | X | X | X | O | O | O | X |
| Claude Sonnet 4.5 (default) | O | O | O | O | X | O | O | X | X | O | X | X | O | O | X | X | X | O | X | O |
| Claude Sonnet 4.5 (max) | O | O | O | O | X | O | O | X | X | O | X | X | O | O | X | O | X | O | X | O |
| K-Exaone 236B (default) | O | ERR | O | O | O | O | ERR | O | ERR | ERR | ERR | ERR | O | O | ERR | O | ERR | O | ERR | O |
| Solar Pro3 (default) | O | X | O | X | O | O | X | X | O | X | X | X | O | X | O | O | X | X | X | X |
</details>

<details>
<summary>MCSAT9 2022</summary>

| Model | Q01 | Q02 | Q03 | Q04 | Q05 | Q06 | Q07 | Q08 | Q09 | Q10 | Q11 | Q12 | Q13 | Q14 | Q15 | Q16 | Q17 | Q18 | Q19 | Q20 |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| GPT-5.3 Codex (high) | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O |
| Gemini 3.1 Pro (default) | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O |
| Gemini 3.1 Pro (xhigh) | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O |
| Grok-4 (default) | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | ERR |
| Grok-4 (max) | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | O | ERR |
| GPT-5.3 Codex (default) | O | O | O | O | X | O | O | O | O | X | O | X | X | O | X | O | O | O | O | O |
| Claude Sonnet 4.5 (default) | O | O | O | O | X | O | O | O | O | X | X | O | X | O | X | X | O | X | O | X |
| Claude Sonnet 4.5 (max) | O | O | O | O | X | O | O | O | O | X | X | X | X | O | X | X | O | X | O | X |
| K-Exaone 236B (default) | O | ERR | O | O | ERR | O | O | O | ERR | O | O | O | O | ERR | O | O | ERR | ERR | O | ERR |
| Solar Pro3 (default) | O | X | X | O | X | O | O | X | X | X | X | X | X | X | O | X | X | O | O | X |
</details>
