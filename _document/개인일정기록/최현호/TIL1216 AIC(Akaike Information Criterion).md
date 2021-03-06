# TIL1216

## (1) AIC (Akaike Information Criterion)

> ref.https://m.blog.naver.com/euleekwon/221465294530
>
> AIC는 주어진 데이터 셋에 대한 통계 모델의 상대적인 품질을 평가는 것이다.
>
> AIC 값은 낮을수록 좋다고 하는데, 왜 낮을수록 좋은지 공식을 통해 알아본다.
>
> 
>
> 모델을 선택하는 방법에는 다양한 방법이 있지만, 모델 선택법 중 하나인 AIC는 **최소의 정보 손실을 갖는 모델이 가장 데이터와 적합한 모델**로 선택되는 방법이다.
>
> *AIC = -2ln(L) + 2k*
>
> 여기서 -2ln(L)은 모형의 적합도를 의미하며, k는 모형의 추정된 파리미터의 개수이다. 다시 -2ln(L)에서 L은 Likelihood function을 의미하며, AIC 값이 낮다는 것은 즉 모형의 적합도가 높은 것을 의미한다. (모형의 적합도 = 실제자료와 연구 모형이 얼마나 부합하는지 적합 정도)
>
> 여기서 2k는 모형의 추정된 파라미터의 개수를 의미하며, 해당 모형에 패널티를 주기 위해 사용한다. 실제로 어떤 모형이 적합도를 높이기 위해 여러 불필요한 파라미터를 사용할 수도 있다. 실제 모형 비교시 독립변수가 많은 모형이 적합도 면에서 유리하게 되는데, 이는 즉 독립변수에 따라서 모형의 적합도에 차이가 난다는 의미이다. 따라서 이를 상쇄시키기 위하여 불필요한 파라미터, 즉 독립변수의 수가 증가할수록 2k를 증가시켜 패널티를 부여하여 모델의 품질을 평가한다.
>
> 따라서 2k가 증가할수록 AIC 값이 증가하게 되므로 좋지 않은 모형이된다고 볼 수 있다.

