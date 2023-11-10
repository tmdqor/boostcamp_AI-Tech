# 경사하강법 (Gradient descent)

## 경사하강법으로 선형회귀 계수 구하기
* 선형회귀 목적식 $ ||y - X\beta||_{2} $ 에서 최소화하는 $ \beta $ 구해야한다
* 목적식을 최소화하는 $ \beta $를 구하는 경사하강법 알고리즘은 다음과 같다.
$$ \beta^{(t+1)} \leftarrow \beta^{(t)} + \frac {\lambda} {n} \frac {X^T(y - X\beta^{(t)})} {||y - X\beta^{(t)}||} $$

```py
train_x = np.array([[1,1,1], [1,1,2], [1,2,2], [2,2,3], [2,3,3], [1,2,3]])
train_y = np.dot(train_x, np.array([1,3,5])) + 7

# random initialize
beta_gd = [9.4, 10.6, -3.7, -1.2]
# 상수항까지 한번에 matrix multiplication으로 계산하기 위해 expand
expand_x = np.array([np.append(x, [1]) for x in train_x])

for t in range(5000):
    pred_y = expand_x @ beta_gd
    error = train_y - pred_y
    # matmul을 통해 gradient를 한번에 계산 (beta_gd의 gradient)
    grad = -np.transpose(expand_x) @ error

    # lr_rate = 0.01
    beta_gd = beta_gd - 0.01 * grad

print("After gradient descent, beta_gd : {}".format(beta_gd))
```

# 확률적 경사하강법(stochastic gradient descent)
* 모든 데이터를 사용해서 업데이트하는 대신 데이터 한개 또는 일부 활용하여 업데이트