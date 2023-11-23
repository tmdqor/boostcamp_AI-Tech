# 학습 회고

## Mon - Day 15
- **Peer-Session**  
    - 지난주의 배웠던 gather에 대해 서로 얘기하며 개념을 잡아갔다.  
    - zero_grad()를 호출해야하는 이유에 대해 PyTorch가 그래디언트를 누적하기 때문이다. 이러한 누적 동작이 RNN(순환 신경망)을 학습할 때나 여러 미니 배치에 걸쳐 손실의 그래디언트를 계산할 때 편리하기에 기본적으로 파이토치는 loss.backward()를 호출할 때마다 그래디언트를 누적하도록 설정되어있다.
- **Fact**  
: 1,2,3 강 강의를 학습하였다. 
- **Feeling**  
: 수업에서 다루지 않은 내용에 의문을 품고 동료들과 같이 개념을 하나씩 쌓아갔다. 피어세션은 점차 발전하는데 개인으로는 어떤지 잘 모르겠다. 월요병인지 오후가 되니 집중력이 많이 떨어졌다. 오늘 회고를 쓰며 반성해본다.
- **Future Plan & Finding**  
: 본격적인 torch 코드가 나와서 해당 코드에 익숙해지며 이전의 수학과 접목해 학습해야겠다.


## Tue - Day 16
- **Peer-Session**  
    - 오늘 배운 내용에 관련하여 서로서로 개념 체크
    - googlenet에서 1x1 conv 을 통해 채널 수를 줄이는 방식이 정보 소실이 되지는 않는다.
    - NLP와 관련된 논문을 읽어보는 것이 좋겠다.
- **Fact**  
: 4,5,6,7 강 강의를 학습하였다. CNN과 RNN에 관해 여러 이론들을 듣고 실습하였다.
- **Feeling**  
: 지금까지 나온 코드들을 하나하나 이해하기도 아직 버겁다. 언젠가 배운 개념과 코드들이 익숙해져서 아이디어를 내 손으로 팍팍 구현하길 바란다. 조금씩 조금씩 좀 더 나아지자. 확실히 어제보단 오늘이 괜찮게 공부한 것 같다 ㅎㅎ
- **Future Plan & Finding**  
: 오늘 배운 것들의 많은 부분들이 Transformer로 대체되고 있다고 한다. 다음 강의인 transformer에 대해 확실히 이해하고 넘어가야겠다. Data Visualization 강의는 코어타임 외에 시간을 할애하여 수강하겠다.


## Wed - Day 17
- **Peer-Session**  
    - transformer에서 encoder 부분 코드 해석
    - NADE와 Autoregressive Model 차이
    - Implicit Method와 Explicit Method 차이
- **Fact**  
: 8, 9 강 강의를 학습하였다. transformer 실습을 통해 code 해석을 하였다.
- **Feeling**  
: transformer 까지는 강의가 어느정도 이해가 됐는데 Generative Models 전반적인 이해가 부족하다. 특히 9강에서 강사님의 설명에 영어의 비율이 올라가면서 이해력이 뚝 떨어졌다. 아직 익숙하지 않은 용어들로 설명하시니 너무 힘들었다.ㅜ 이 분야에서 다 쓰는 용어들이지만 어우.. 벅찬 하루다. 익숙해져야지..
- **Future Plan & Finding**  
: transformer와 이번주 실습에 나온 모든 code 복습을 하면서 정리해야겠다. 그 후 심화과제도 풀어야겠다.


## Thu - Day 18
- **Peer-Session**  
    - 기본과제 공부하며 분석한 코드 해석 공유
    - masked_fill(mask, value) 함수 조사
        - mask (*BoolTensor*) – the boolean mask
        - value (float) – the value to fill in with
    - Multi-Head Attention 이 어떻게 Transformer가 다른 Position들에 대해 집중할 수 있게 해주는가?**
    (Multi-headed attention (MHA) allows Transformer to focus on different positions.)

- **Fact**  
: 기본과제 1~5 수행과 코드 분석 및 해석
- **Feeling**  
: 과제의 코드를 하나하나씩 뜯어보며 이론과 비교하며 분석해보았다. RNN과 Transformer는 아직 완전히 이해가 되진 않았지만 계속 보다보면 늘겠지라는 마음으로 보고있다. 점점 피어세션의 질이 높아지는 것을 느낀다. 예전에는 시간이 남았는데 오늘은 오히려 조금 부족하다. 마지막 퀴즈도 풀었는데 코드 분석과 다르게 이론적으로는 많이 부족함을 느낀다.
- **Future Plan & Finding**  
: 심화과제까지 풀려고 했으나 기본과제 코드 분석이 생각보다 오래 걸렸다. 심화과제와 Position embedding 실습 코드도 봐야겠다. 코어타임 전에 Data Visualization 을 다 들어야놓고, 코어타임에는 온전히 코드에 집중해보겠다.


## Fri - Day 19
- **Fact**  
: 
- **Feeling**  
: 
- **Future Plan & Finding**  
: 



