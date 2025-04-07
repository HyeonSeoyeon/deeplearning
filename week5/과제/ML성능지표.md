# 혼동 행렬 (Confusion Matrix)
- TP (True Positive): 긍정을 긍정으로 올바르게 예측
- TN (True Nagative): 부정을 부정으로 올바르게 예측
- FN (False Negative): 부정을 긍정으로 잘못 예측
- FP (False Positive): 긍정을 부정으로 잘못 예측

### 예)
- 입력: 남자 ; 결과: 남자 -> TP
- 입력: 여자 ; 결과: 여자 -> TN
- 입력: 남자 ; 결과: 여자 -> FN
- 입력: 여자 ; 결과: 남자 -> FP

---


# 성능지표
1. ***Sensitive(민감도) = Recall***
- ***Sensitivity = TP / (FN+TP) (= Recall)***
- 정답(입력)인 긍정 중에서, 제대로 맞힌 비율
- -> 높을수록 진짜 긍정을 잘 골라냄

2. ***Specificity(특이도)***
- ***Specificity = TN/ (FP+TN)***
- 정답(입력)인 부정 중에서, 제대로 맞힌 비율
- -> 높을수록 부정을 잘 골라냄

3. ***Precision(정밀도)***
- ***Precision = TP/ (TP+FP)***
- 결과가 긍정이라고 한 것 중에 진짜 긍정인 비율
- -> 예측이 얼마나 "정확하게 긍정"인지 보는 지표

4. ***Recall(재현율)***
- ***Recall = TP / (FN+TP)***
- 정답(입력) 중에서 얼마나 잘 찾았는가?

5. ***F1 score***
- ***F1 score = 2 * (precision * recall) / (precision + recall)***
- Precision과 Recall의 조화 평균으로, 정밀도와 재현율(민감도)을 균형있게 평가하는 지표.


---

## 요약

### Recall	
- 놓치지 않고 잘 찾았나? (실제 긍정 중 맞힌 비율)	
- ```TP / (TP + FN)```

### Precision
- 예측이 얼마나 정확했나? (예측한 긍정 중 진짜 비율)
- ```TP / (TP + FP)```

### Specificity
- 부정을 얼마나 잘 걸러냈나?	
- ```TN / (TN + FP)```

### F1 Score	
- Recall과 Precision의 균형	
- ```2 * (P × R) / (P + R)```
