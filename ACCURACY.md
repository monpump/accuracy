# NAVIGATE Public Accuracy Ledger

Independent daily recomputation of AI prediction accuracy from `data/tracking/signal_log.parquet`. Produced by the cloud /schedule routine `NAVIGATE Public Accuracy Ledger` (KST 09:00 mon-sat) running in Anthropic's environment, separate from the local daemon. This is the public record behind the **AI 정확도 매일 공개** guarantee.

Methodology: only predictions with |direction| >= 0.05 (clear call, not 관망) and a verified actual return are counted. Agent stats require n>=5 samples in the window.

---

## 2026-05-13 09:00 KST (independent cloud audit)

- 7-day: 12/19 judged = **63.2%**
- 30-day: 48/65 judged = **73.8%**
- All-time: 65/90 judged = **72.2%**

### Per market (last 30d)
  - DIA: 10/16 = 62.5%
  - KOSDAQ: 7/8 = 87.5%
  - KOSPI: 14/16 = 87.5%
  - QQQ: 8/11 = 72.7%
  - SPY: 9/14 = 64.3%

### Top 5 agents (last 30d, n>=5)
  - derivatives_analyst: 82.8% (n=29)
  - academic_research: 82.8% (n=29)
  - bayesian_fusion_predictor: 80.0% (n=40)
  - debate_moderator: 76.9% (n=26)
  - wavelet_analyst: 75.0% (n=44)

### Bottom 3 agents (last 30d, n>=5)
  - rnd_analyst: 40.9% (n=22)
  - scenario_war_room: 34.2% (n=38)
  - risk_manager: 24.6% (n=65)

## 2026-05-12 09:00 KST (independent cloud audit)

- 7-day: 13/19 judged = **68.4%**
- 30-day: 52/67 judged = **77.6%**
- All-time: 65/87 judged = **74.7%**

### Per market (last 30d)
  - DIA: 11/17 = 64.7%
  - KOSDAQ: 8/9 = 88.9%
  - KOSPI: 14/16 = 87.5%
  - QQQ: 9/11 = 81.8%
  - SPY: 10/14 = 71.4%

### Top 5 agents (last 30d, n>=5)
  - academic_research: 86.7% (n=30)
  - bayesian_fusion_predictor: 85.7% (n=42)
  - derivatives_analyst: 84.8% (n=33)
  - debate_moderator: 82.1% (n=28)
  - wavelet_analyst: 80.4% (n=46)

### Bottom 3 agents (last 30d, n>=5)
  - rnd_analyst: 35.0% (n=20)
  - scenario_war_room: 30.6% (n=36)
  - risk_manager: 20.9% (n=67)

## 2026-05-11 15:05 KST (independent cloud audit)

- 7-day: 10/15 judged = **66.7%**
- 30-day: 46/60 judged = **76.7%**
- All-time: 59/80 judged = **73.8%**

### Per market (last 30d)
  - DIA: 10/16 = 62.5%
  - KOSDAQ: 8/8 = 100.0%
  - KOSPI: 12/14 = 85.7%
  - QQQ: 7/9 = 77.8%
  - SPY: 9/13 = 69.2%

### Top 5 agents (last 30d, n>=5)
  - academic_research: 85.7% (n=28)
  - bayesian_fusion_predictor: 85.0% (n=40)
  - derivatives_analyst: 84.4% (n=32)
  - debate_moderator: 81.5% (n=27)
  - wavelet_analyst: 79.5% (n=44)

### Bottom 3 agents (last 30d, n>=5)
  - rnd_analyst: 36.8% (n=19)
  - scenario_war_room: 32.4% (n=34)
  - risk_manager: 21.7% (n=60)

## 2026-05-04 23:18 KST (independent cloud audit)

- 7-day: 9/13 judged = **69.2%**
- 30-day: 44/58 judged = **75.9%**
- All-time: 48/64 judged = **75.0%**

### Per market (last 30d)
  - DIA: 9/12 = 75.0%
  - KOSDAQ: 8/10 = 80.0%
  - KOSPI: 9/13 = 69.2%
  - QQQ: 9/11 = 81.8%
  - SPY: 9/12 = 75.0%

### Top 5 agents (last 30d, n>=5)
  - derivatives_analyst: 85.7% (n=42)
  - wavelet_analyst: 83.0% (n=47)
  - fundamental_analyst: 81.8% (n=44)
  - academic_research: 80.8% (n=26)
  - ensemble_predictor: 79.6% (n=49)

### Bottom 3 agents (last 30d, n>=5)
  - rnd_analyst: 25.0% (n=8)
  - scenario_war_room: 20.6% (n=34)
  - risk_manager: 13.8% (n=58)

## 2026-05-04 22:43 KST (independent cloud audit)

- 7-day: 9/13 judged = **69.2%**
- 30-day: 48/63 judged = **76.2%**
- All-time: 52/69 judged = **75.4%**

### Per market (last 30d)
  - DIA: 9/13 = 69.2%
  - KOSDAQ: 9/11 = 81.8%
  - KOSPI: 10/14 = 71.4%
  - QQQ: 10/12 = 83.3%
  - SPY: 10/13 = 76.9%

### Top 5 agents (last 30d, n>=5)
  - derivatives_analyst: 85.7% (n=42)
  - wavelet_analyst: 83.0% (n=47)
  - fundamental_analyst: 81.8% (n=44)
  - academic_research: 80.8% (n=26)
  - ensemble_predictor: 79.6% (n=49)

### Bottom 3 agents (last 30d, n>=5)
  - rnd_analyst: 25.0% (n=8)
  - scenario_war_room: 20.6% (n=34)
  - risk_manager: 14.3% (n=63)

