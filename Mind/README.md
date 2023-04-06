인공 감정, 개성, 등 내부 변수를 조절하는 코드를 구현해봅니다

# 인공 감정

### 1차 서치

- Emotion Model Based Chatbot: 감정 모델 기반의 챗봇 구현 github
https://github.com/simonlee1004/emotionalchatbot

- AI DEV 인공지능 개발자 모임 게사판 사이트
http://aidev.co.kr/aemotion/486


인공 감정 (Artificial Emotion)은 AI agent에게 가상적으로 감정을 부여하려는 시도이다. AI agent에게 감정이 왜 필요한가? 인간과의 정서적인 상호작용을 위해서이다. 인간과 인간과의 대화를 생각하면, 우리는 대화를 할때 상대의 리액션 또한 중요하게 생각한다. ChatGPT와 같이 훌륭한 챗봇 시스템도 결국엔 아주 좋은 사전과 얘기하는 듯한 느낌까지만 줄 수 있을 뿐이다.

영화 HER (2013)의 그녀를 목표로 한다면 필요한 요소이다.
또한 Nier Automata (2017)를 생각하면 감정은 AI에게 행동 목표를 부여하는데에 효과적일것이다.

딥러닝이 부상하기 이전에는 알고리즘적으로 Game AI를 구현하려는 시도중에 인공감정에 대한 연구도 있었던 것 같다. 내가 자세히 다 알아보지는 않았지만, 그 계보가 끊기지 않았나 싶다.

### 전제

#### 1. 감성(Affect)은 Emotion, Mood, Feeling 3가지로 이루어져 있다. 그리고 Personality 와의 상호 업데이트가 있다.

![image](https://user-images.githubusercontent.com/45591887/230360803-0c022312-b0e3-439d-9eae-6895011be43f.png)

출처: https://www.youtube.com/watch?v=8D_YNXqTDTs


#### 2. Mood는 내부 Vector, Feeling은 외부 Vector, Emotion은 현재 State 이다.

![image](https://user-images.githubusercontent.com/45591887/230361001-cc542baa-f708-47b3-9f17-66985b5df950.png)

폴 에크만을 비롯한 심리학자들이 말하는 Emotion 들을 살펴보면,

Neutral, Happiness, Sadness, Surprise, Anger, Fear, Disgust

와 같은 종류가 있다. Happiness를 살펴보면, 어떤 자극에 대한 행복한 Feeling이 있을 수 있고 그로 인한 행복한 Emotion State가 있을수가 있을 것이다.


#### 3. Emotion은 N차원의 공간에 정의되고, Feeling, Mood는 그 방향으로 가는 벡터인가?

![3](https://user-images.githubusercontent.com/45591887/230366072-6d56bec4-2607-4c66-a095-ae386a8204ab.PNG)


이것은 감정간의 Transition 을 고려할 필요가 있다.

불행한 상태에 행복 벡터를 주입하면, 중립을 거치지 않고 행복해질수가 있는가?

감정 A  ->  감정 B 의  Transition 상태에서 다른 감정이 나타나는가?

Research 시작








