인공 감정, 개성, 등 내부 변수를 조절하는 코드를 구현해봅니다

# 인공 감정

1차 서치

- Emotion Model Based Chatbot: 감정 모델 기반의 챗봇 구현 github
https://github.com/simonlee1004/emotionalchatbot

- AI DEV 인공지능 개발자 모임 게사판 사이트
http://aidev.co.kr/aemotion/486


인공 감정 (Artificial Emotion)은 AI agent에게 가상적으로 감정을 부여하려는 시도이다. AI agent에게 감정이 왜 필요한가? 인간과의 정서적인 상호작용을 위해서이다. 인간과 인간과의 대화를 생각하면, 우리는 대화를 할때 상대의 리액션 또한 중요하게 생각한다. ChatGPT와 같이 훌륭한 챗봇 시스템도 결국엔 아주 좋은 사전과 얘기하는 듯한 느낌까지만 줄 수 있을 뿐이다.

영화 HER (2013)의 그녀를 목표로 한다면 필요한 요소이다.
또한 Nier Automata (2017)를 생각하면 감정은 AI에게 행동 목표를 부여하는데에 효과적일것이다.

딥러닝이 부상하기 이전에는 알고리즘적으로 Game AI를 구현하려는 시도중에 인공감정에 대한 연구도 있었던 것 같다. 내가 자세히 다 알아보지는 않았지만, 그 계보가 끊기지 않았나 싶다.

### 전제

감정은 Emotion, Mood, Personality, Feeling 4가지로 이루어져 있다.
![image](https://user-images.githubusercontent.com/45591887/230360803-0c022312-b0e3-439d-9eae-6895011be43f.png)

출처: https://www.youtube.com/watch?v=8D_YNXqTDTs
