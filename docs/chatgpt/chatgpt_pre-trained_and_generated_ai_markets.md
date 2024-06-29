# ChatGPT Pre-trained and Generated AI Markets

목표:

- ChatGPT가 거치는 3단계 훈련 과정에 대해 설명할 수 있다.
- 다양한 생성형 AI의 종류와 생성 AI 마켓 트렌드를 파악할 수 있다.

## ChatGPT Pre-trained

ChatGPT 는 인공신경망의 자동 훈련 뿐만아니라 더 좋은 답안에 대한 인간 사용자 피드백 기반 강화 학습(RLHF, Reinforcement Learning from Human Feedback)을 거쳐 파인튜닝(fine- tuning)되었다. 이러한 훈련 과정을 거치는데 매우 많은 시간과 자원이 투입된다.

> [!NOTE]
>
> - G: Generative
> - P: Pre-trained
> - T: Transformer

![ChatGPT pre-trained](/assets/images/chatgpt_pre_trained.png)

1. Pre-training Language Model
   - 무수한 데이터로부터 인공신경망이 방대한 딥러닝 학습한다.
   - 언어 모델이 만들어 진다.
   - 지식을 학습한 것이다.
2. Reward Model
   - 1단계로 나오는 여러 결과물에 대해 사람(instructor)이 채점해서 "좋은 답변"의 정도를 점수화 해준다.
   - 적은 파라미터를 갖고도 더 좋은 답변을 할 수 있게 한다.
   - 많은 사람들의 채점하고 자료가 쌓이면 좋다 나쁘다의 패턴이 발생하고 이를 톡립시켜 평가 인공지능으로 만든다.
3. Fine-tuning with Reinforcement Learning
   - RLHF 시스템에서 모델이 생성한 텍스트를 사람이 어느 정도 "좋다"고 생각할지 추정하여 답변 품질을 조정한다.
   - 자가 발전 한다. 사람이 필요 없다.
   - 명령이 입력되면 1단계의 학습한 결과 모델을 토대로 답변을 만들고 2단계의 사람이 채점한 결과를 토대로 만들어진 평가 인공지능에게 채점한다.
   - 채점 후, 이를 새로운 지식으로 받아드리고 새로운 모델을 만들고 이전 모델을 결부 시켜 다시 평가 인공지능에게 채점한다. 위와 반복된다.

> [!NOTE]
> 1단계에서 파라미터가 많다고 좋은 AI 라고 말하기 어렵다. 왜냐하면 2단계, 3단계가 있기 때문이다.
> 1단계에서 어떤 내용을 학습했는가, 2단계에서 인간으로부터 어떤 피드백을 받았는가에 따라 언제든 더 좋은 AI 가 등장할 수 있다.

자세한 내용은 [공식 페이지](https://openai.com/index/chatgpt/) 에서 확인할 수 있습니다.

## Generative AI types and market trends

생성현 AI 의 종류는 다양하다:

- 텍스트, 음성, 이미지, 동영상, 음악 등 형식이 다양해도 0과 1로 디지털화된 결과물은 동일한 방식을 적용해 생성할 수 있다.

> [!NOTE]
> T2I: Text to Image

생성 AI 마켓 트랜드:

- OpenAI:
- Hugging Face:
- Jasper:
- stability.ai: 이미지 생성

> [!NOTE]
> AI 산업: Text > Image > Video > ... > Code
