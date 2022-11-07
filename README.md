# ML-math

- 사이킷런에 사용할 훈련 세트는 2차원 배열이어야해요.

- perch_length, perch_weight 배열이 있을시에 
from sklearn.model_selection import train_test_split

train_input, test_input, train_target, test_target = train_test_split(
    perch_length, perch_weight, random_state = 42
)
train_input = train_input.reshape(-1,1)
test_input = test_input.reshape(-1,1)

이렇게 할텐데, 이때 length 는 입력, weight는 타겟(정답) 으로 나눠서 생각하면 편해요.
