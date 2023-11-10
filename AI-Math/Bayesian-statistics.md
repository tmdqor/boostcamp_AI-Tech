# 베이즈 통계학 (Bayesian statistics)

## 조건부 확률(Conditional probability)
* 사건 $B$가 일어났을 때, 사건 $A$ 가 발생할 확률

$$ P(A|B) = \frac {P(A \cap B)} {P(B)}, 단, P(B) > 0 $$

## 베이즈 정리
* 두 확률 변수의 사전 확률과 사후 확률 사이의 관계를 나타내는 정리
* 사전확률과 가능도를 안다면 사후확률을 알 수 있다
$$ P(\theta|D) = P(\theta) \frac {P(D|\theta)} {P(D)} $$
$$사후확률 (posterior) = 사전확률 (prior) \frac {가능도 (likelihood)} {관측데이터(Evidence)}$$

* 사전 확률 ( Prior Probability ) : 현재 가지고 있는 정보를 기초로하여 정한 초기 확률
* 사후 확률 ( Posteriori Probability) : 사건 발생 후에 어떤 원인으로부터 일어난 것이라고 생각되어지는 확률
* 가능도(Likelihood, 우도:尤度) : 원인(θ)이 발생했다는 가정하에 결과(D)가 발생할 확률
* 관측데이터(Evidence) : 해당 결과가 나오도록 모든 원인들 마다 기여하는 확률들의 합


# 조건부확률과 인과관계
* 조건부 확률은 유용한 통계적 해석을 제공하지만, 인과관계(Causality)를 추론할 때 함부로 사용해서는 안된다. 데이터가 아무리 많아져도 조건부 확률만을 가지고 인과관계를 추론하는 것은 불가능하다.

