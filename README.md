# CSAT Economics Model Performance Report

Static snapshot of an interactive analysis comparing how different LLMs (GPT, Claude, Gemini, Grok, Solar, EXAONE, ...) perform on Korean CSAT (수능) economics exam questions: accuracy, cost, response speed, and error breakdowns.

## Model Leaderboard

| Rank | Model | Composite Index | Overall Pass@1 (%) | Valid-Response Pass@1 (%) | Error Rate (%) | Cost (USD) | Avg Response Time (s) |
|---|---|---|---|---|---|---|---|
| 1 | GPT-5.3 Codex (high) | 100.0 | 100.0 | 100.0 | 0.0 | 5.264 | 15.4 |
| 2 | Gemini 3.1 Pro (default) | 99.7 | 99.7 | 99.7 | 0.0 | 7.962 | 15.2 |
| 3 | Gemini 3.1 Pro (xhigh) | 99.3 | 99.3 | 99.3 | 0.0 | 8.087 | 16.0 |
| 4 | Grok-4 (default) | 87.1 | 92.7 | 98.9 | 6.3 | 15.848 | 72.3 |
| 5 | Grok-4 (max) | 86.2 | 91.7 | 97.9 | 6.3 | 15.727 | 68.9 |
| 6 | GPT-5.3 Codex (default) | 54.3 | 54.3 | 54.3 | 0.0 | 0.508 | 1.4 |
| 7 | Claude Sonnet 4.5 (default) | 53.3 | 53.3 | 53.3 | 0.0 | 1.223 | 2.3 |
| 8 | Claude Sonnet 4.5 (max) | 52.3 | 52.3 | 52.3 | 0.0 | 1.236 | 2.2 |
| 9 | K-Exaone 236B (default) | 49.9 | 66.3 | 99.0 | 33.0 | 0.796 | 115.8 |
| 10 | Solar Pro3 (default) | 40.7 | 40.7 | 40.7 | 0.0 | 0.159 | 5.3 |

## 2. Score Performance By Points

### Model by point-value heatmap: Overall Pass@1 (%)

|  | 2 pt | 3 pt |
|---|---|---|
| GPT-5.3 Codex (high) | 100 | 100 |
| Gemini 3.1 Pro (default) | 100 | 99.33 |
| Gemini 3.1 Pro (xhigh) | 99.33 | 99.33 |
| Grok-4 (default) | 94.00 | 91.33 |
| Grok-4 (max) | 92.67 | 90.67 |
| GPT-5.3 Codex (default) | 54.67 | 54.00 |
| Claude Sonnet 4.5 (default) | 57.33 | 49.33 |
| Claude Sonnet 4.5 (max) | 56.67 | 48.00 |
| K-Exaone 236B (default) | 64.00 | 68.67 |
| Solar Pro3 (default) | 46.67 | 34.67 |

### Model by point-value heatmap: Valid-Response Pass@1 (%)

|  | 2 pt | 3 pt |
|---|---|---|
| GPT-5.3 Codex (high) | 100 | 100 |
| Gemini 3.1 Pro (default) | 100 | 99.33 |
| Gemini 3.1 Pro (xhigh) | 99.33 | 99.33 |
| Grok-4 (default) | 99.30 | 98.56 |
| Grok-4 (max) | 98.58 | 97.14 |
| GPT-5.3 Codex (default) | 54.67 | 54.00 |
| Claude Sonnet 4.5 (default) | 57.33 | 49.33 |
| Claude Sonnet 4.5 (max) | 56.67 | 48.00 |
| K-Exaone 236B (default) | 98.97 | 99.04 |
| Solar Pro3 (default) | 46.67 | 34.67 |

## 3. Score Performance By Image Presence

### Model by image-presence heatmap: Overall Pass@1 (%)

|  | No Image | Image |
|---|---|---|
| GPT-5.3 Codex (high) | 100 | 100 |
| Gemini 3.1 Pro (default) | 100 | 99.13 |
| Gemini 3.1 Pro (xhigh) | 99.46 | 99.13 |
| Grok-4 (default) | 92.43 | 93.04 |
| Grok-4 (max) | 93.51 | 88.70 |
| GPT-5.3 Codex (default) | 51.89 | 58.26 |
| Claude Sonnet 4.5 (default) | 54.05 | 52.17 |
| Claude Sonnet 4.5 (max) | 52.43 | 52.17 |
| K-Exaone 236B (default) | 66.49 | 66.09 |
| Solar Pro3 (default) | 42.16 | 38.26 |

### Model by image-presence heatmap: Valid-Response Pass@1 (%)

|  | No Image | Image |
|---|---|---|
| GPT-5.3 Codex (high) | 100 | 100 |
| Gemini 3.1 Pro (default) | 100 | 99.13 |
| Gemini 3.1 Pro (xhigh) | 99.46 | 99.13 |
| Grok-4 (default) | 98.28 | 100 |
| Grok-4 (max) | 97.74 | 98.08 |
| GPT-5.3 Codex (default) | 51.89 | 58.26 |
| Claude Sonnet 4.5 (default) | 54.05 | 52.17 |
| Claude Sonnet 4.5 (max) | 52.43 | 52.17 |
| K-Exaone 236B (default) | 99.19 | 98.70 |
| Solar Pro3 (default) | 42.16 | 38.26 |

## 4. Point Value x Image Presence

### Model by point-image segment heatmap: Overall Pass@1 (%)

|  | 2 pt / Image | 2 pt / No Image | 3 pt / Image | 3 pt / No Image |
|---|---|---|---|---|
| GPT-5.3 Codex (high) | 100 | 100 | 100 | 100 |
| Gemini 3.1 Pro (default) | 100 | 100 | 98.18 | 100 |
| Gemini 3.1 Pro (xhigh) | 100 | 98.89 | 98.18 | 100 |
| Grok-4 (default) | 93.33 | 94.44 | 92.73 | 90.53 |
| Grok-4 (max) | 86.67 | 96.67 | 90.91 | 90.53 |
| GPT-5.3 Codex (default) | 55.00 | 54.44 | 61.82 | 49.47 |
| Claude Sonnet 4.5 (default) | 50.00 | 62.22 | 54.55 | 46.32 |
| Claude Sonnet 4.5 (max) | 48.33 | 62.22 | 56.36 | 43.16 |
| K-Exaone 236B (default) | 60.00 | 66.67 | 72.73 | 66.32 |
| Solar Pro3 (default) | 40.00 | 51.11 | 36.36 | 33.68 |

### Model by point-image segment heatmap: Valid-Response Pass@1 (%)

|  | 2 pt / Image | 2 pt / No Image | 3 pt / Image | 3 pt / No Image |
|---|---|---|---|---|
| GPT-5.3 Codex (high) | 100 | 100 | 100 | 100 |
| Gemini 3.1 Pro (default) | 100 | 100 | 98.18 | 100 |
| Gemini 3.1 Pro (xhigh) | 100 | 98.89 | 98.18 | 100 |
| Grok-4 (default) | 100 | 98.84 | 100 | 97.73 |
| Grok-4 (max) | 98.11 | 98.86 | 98.04 | 96.63 |
| GPT-5.3 Codex (default) | 55.00 | 54.44 | 61.82 | 49.47 |
| Claude Sonnet 4.5 (default) | 50.00 | 62.22 | 54.55 | 46.32 |
| Claude Sonnet 4.5 (max) | 48.33 | 62.22 | 56.36 | 43.16 |
| K-Exaone 236B (default) | 97.30 | 100 | 100 | 98.44 |
| Solar Pro3 (default) | 40.00 | 51.11 | 36.36 | 33.68 |

## 5. Cost And Speed

![Total cost vs average response time](images/cost_speed.png)

## 6. Error Analysis

### API error count by model (cases)

| Model | Errors |
|---|---|
| Solar Pro3 (default) | 0 cases |
| Claude Sonnet 4.5 (max) | 0 cases |
| Claude Sonnet 4.5 (default) | 0 cases |
| GPT-5.3 Codex (default) | 0 cases |
| Gemini 3.1 Pro (xhigh) | 0 cases |
| Gemini 3.1 Pro (default) | 0 cases |
| GPT-5.3 Codex (high) | 0 cases |
| Grok-4 (max) | 19 cases |
| Grok-4 (default) | 19 cases |
| K-Exaone 236B (default) | 99 cases |

## 7. Additional Analysis By Difficulty

### Model by difficulty heatmap: Overall Pass@1 (%)

|  | Low difficulty | Medium difficulty | High difficulty |
|---|---|---|---|
| GPT-5.3 Codex (high) | 100 | 100 | 100 |
| Gemini 3.1 Pro (default) | 100 | 100 | 66.67 |
| Gemini 3.1 Pro (xhigh) | 100 | 100 | 33.33 |
| Grok-4 (default) | 95.95 | 90.32 | 0.00 |
| Grok-4 (max) | 95.95 | 87.90 | 0.00 |
| GPT-5.3 Codex (default) | 81.50 | 17.74 | 0.00 |
| Claude Sonnet 4.5 (default) | 87.28 | 7.26 | 0.00 |
| Claude Sonnet 4.5 (max) | 87.28 | 4.84 | 0.00 |
| K-Exaone 236B (default) | 79.19 | 50.00 | 0.00 |
| Solar Pro3 (default) | 56.65 | 19.35 | 0.00 |

## 8. Problem-Level Correctness Views

### Model accuracy by exam type: Overall Pass@1 (%)

|  | CSAT 2026 | CSAT | MCSAT6 | MCSAT9 |
|---|---|---|---|---|
| GPT-5.3 Codex (high) | 100 | 100 | 100 | 100 |
| Gemini 3.1 Pro (default) | 100 | 100 | 99.00 | 100 |
| Gemini 3.1 Pro (xhigh) | 100 | 100 | 99.00 | 99.00 |
| Grok-4 (default) | 100 | 100 | 98.94 | 97.83 |
| Grok-4 (max) | 95.00 | 98.94 | 96.77 | 97.87 |
| GPT-5.3 Codex (default) | 45.00 | 45.00 | 63.00 | 55.00 |
| Claude Sonnet 4.5 (default) | 45.00 | 45.00 | 63.00 | 52.00 |
| Claude Sonnet 4.5 (max) | 45.00 | 45.00 | 58.00 | 54.00 |
| K-Exaone 236B (default) | 85.71 | 96.61 | 100 | 100 |
| Solar Pro3 (default) | 45.00 | 39.00 | 44.00 | 39.00 |

### 2 pt / No Image: Overall Pass@1 (%)

|  | CSAT | MCSAT6 | MCSAT9 |
|---|---|---|---|
| GPT-5.3 Codex (high) | 100 | 100 | 100 |
| Gemini 3.1 Pro (default) | 100 | 100 | 100 |
| Gemini 3.1 Pro (xhigh) | 100 | 100 | 96.30 |
| Grok-4 (default) | 100 | 100 | 96.00 |
| Grok-4 (max) | 100 | 100 | 96.15 |
| GPT-5.3 Codex (default) | 51.43 | 64.29 | 48.15 |
| Claude Sonnet 4.5 (default) | 57.14 | 67.86 | 62.96 |
| Claude Sonnet 4.5 (max) | 60.00 | 60.71 | 66.67 |
| K-Exaone 236B (default) | 100 | 100 | 100 |
| Solar Pro3 (default) | 45.71 | 57.14 | 51.85 |

### 2 pt / Image: Overall Pass@1 (%)

|  | CSAT | MCSAT6 | MCSAT9 |
|---|---|---|---|
| GPT-5.3 Codex (high) | 100 | 100 | 100 |
| Gemini 3.1 Pro (default) | 100 | 100 | 100 |
| Gemini 3.1 Pro (xhigh) | 100 | 100 | 100 |
| Grok-4 (default) | 100 | 100 | 100 |
| Grok-4 (max) | 91.67 | 100 | 100 |
| GPT-5.3 Codex (default) | 26.67 | 72.73 | 56.52 |
| Claude Sonnet 4.5 (default) | 33.33 | 72.73 | 39.13 |
| Claude Sonnet 4.5 (max) | 26.67 | 72.73 | 39.13 |
| K-Exaone 236B (default) | 87.50 | 100 | 100 |
| Solar Pro3 (default) | 40.00 | 40.91 | 39.13 |

### 3 pt / No Image: Overall Pass@1 (%)

|  | CSAT | MCSAT6 | MCSAT9 |
|---|---|---|---|
| GPT-5.3 Codex (high) | 100 | 100 | 100 |
| Gemini 3.1 Pro (default) | 100 | 100 | 100 |
| Gemini 3.1 Pro (xhigh) | 100 | 100 | 100 |
| Grok-4 (default) | 100 | 95.83 | 96.88 |
| Grok-4 (max) | 100 | 92.00 | 96.97 |
| GPT-5.3 Codex (default) | 38.24 | 51.85 | 58.82 |
| Claude Sonnet 4.5 (default) | 38.24 | 55.56 | 47.06 |
| Claude Sonnet 4.5 (max) | 35.29 | 44.44 | 50.00 |
| K-Exaone 236B (default) | 95.24 | 100 | 100 |
| Solar Pro3 (default) | 35.29 | 37.04 | 29.41 |

### 3 pt / Image: Overall Pass@1 (%)

|  | CSAT | MCSAT6 | MCSAT9 |
|---|---|---|---|
| GPT-5.3 Codex (high) | 100 | 100 | 100 |
| Gemini 3.1 Pro (default) | 100 | 95.65 | 100 |
| Gemini 3.1 Pro (xhigh) | 100 | 95.65 | 100 |
| Grok-4 (default) | 100 | 100 | 100 |
| Grok-4 (max) | 100 | 95.24 | 100 |
| GPT-5.3 Codex (default) | 62.50 | 65.22 | 56.25 |
| Claude Sonnet 4.5 (default) | 43.75 | 56.52 | 62.50 |
| Claude Sonnet 4.5 (max) | 50.00 | 56.52 | 62.50 |
| K-Exaone 236B (default) | 100 | 100 | 100 |
| Solar Pro3 (default) | 31.25 | 39.13 | 37.50 |

### Model accuracy by category: Overall Pass@1 (%)

|  | Finance | General Economics | International Economics | Macroeconomics | Microeconomics |
|---|---|---|---|---|---|
| GPT-5.3 Codex (high) | 100 | 100 | 100 | 100 | 100 |
| Gemini 3.1 Pro (default) | 100 | 100 | 100 | 98.80 | 100 |
| Gemini 3.1 Pro (xhigh) | 100 | 100 | 98.31 | 98.80 | 100 |
| Grok-4 (default) | 100 | 96.55 | 96.23 | 100 | 100 |
| Grok-4 (max) | 100 | 93.94 | 94.34 | 100 | 98.85 |
| GPT-5.3 Codex (default) | 50.00 | 73.53 | 42.37 | 61.45 | 50.00 |
| Claude Sonnet 4.5 (default) | 53.33 | 67.65 | 28.81 | 63.86 | 54.26 |
| Claude Sonnet 4.5 (max) | 50.00 | 79.41 | 27.12 | 59.04 | 53.19 |
| K-Exaone 236B (default) | 100 | 100 | 96.67 | 100 | 98.31 |
| Solar Pro3 (default) | 33.33 | 58.82 | 27.12 | 46.99 | 39.36 |

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
