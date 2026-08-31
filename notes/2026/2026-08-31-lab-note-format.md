---
date: 2026-08-31
project: transmitter-switching
status: completed
dataset: in-vivo-v1
commit: a13f9c2
config: configs/fitting/h1_baseline.yaml
related_decisions: [D001, D002]
---

# 오늘의 질문

Spike-triggered depletion을 포함한 R dynamics가 synthetic train에서
예상된 within-train depression과 recovery를 만드는가?

# 오늘의 완료조건

- R이 항상 0–1 범위에 있을 것
- 자극이 없을 때 R이 1로 회복할 것
- refill이 느릴수록 late/early ratio가 감소할 것
- recovery interval이 길수록 test response가 회복될 것

# 입력

- Simulation protocol:
- Parameter set:
- Random seed:
- Relevant files:

# 수행한 작업

1. Event-driven depletion jump 구현
2. 5, 20, 40 Hz simulation
3. tau_R sensitivity 확인
4. Sensor convolution 전후 결과 비교

# 결과

## 관찰

- 40 Hz에서 latent release per spike가 감소했다.
- Sensor-filtered fluorescence peak는 동일한 비율로 감소하지 않았다.
- tau_R과 initial release probability 사이에 trade-off가 나타났다.

## 해석

Fluorescence peak만으로 depletion 크기를 직접 추정하기 어렵다.
AUC, early/late ratio와 recovery response를 함께 사용해야 한다.

# 실패·문제

- 첫 spike 직후 R이 음수가 되는 parameter 조건 발견
- Solver tolerance에 따라 peak time이 달라짐

# 다음 조치

- R update를 bounded form으로 수정
- limiting-case unit test 추가
- synthetic recovery에서 tau_R identifiability 확인

# Decision 후보

Observation metric을 peak 단독에서
`peak + AUC + early/late + recovery`로 변경할지 검토한다.
결정 시 D003을 작성한다.
