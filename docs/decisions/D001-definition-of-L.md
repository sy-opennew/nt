# D001: L의 정의

- Date: 2026-11-01
- Status: Accepted
- Owner: 본인
- Approved by: 지도교수
- Related commit: 41bc9e7

## Context

현재 데이터는 LDCV recruitment/activation과 available LDCV pool의
depletion을 각각 식별하기에 충분하지 않다.

## Decision

L은 calcium-dependent LDCV recruitment/competence state로 정의한다.
LDCV pool의 개수로 해석하지 않는다.

## Alternatives considered

1. L을 available LDCV pool로 정의
2. Recruitment state와 pool을 별도 변수로 사용
3. LDCV branch를 완전히 phenomenological filter로 표현

## Rationale

두 개의 LDCV 상태를 추가하면 현재 관측자료에서 식별 가능성이 낮고,
release sink를 포함할 근거도 부족하다. 최소모델에서는 recruitment만
표현하는 것이 주장 범위와 일치한다.

## Consequences

- 기본 L 식에는 peptide release에 의한 depletion sink를 넣지 않는다.
- LDCV depletion이나 pool size에 관한 주장을 하지 않는다.
- r_P는 L과 high-threshold calcium function에 의존한다.

## What would overturn this decision?

- Direct LDCV pool 또는 fusion measurement 확보
- 반복 자극에서 독립적인 LDCV depletion/recovery signature 관측
- One-state model의 systematic predictive failure

## Revisit no later than

M12 prediction lock
