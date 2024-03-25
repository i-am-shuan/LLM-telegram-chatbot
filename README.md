# LLM-telegram-chatbot
- ChatGPT로 질의응답 및 DALLE.2 모델기반 그림을 그려주는 AI 챗봇
<p align="center">
	<img alt="image" src="https://github.com/i-am-shuan/LLM-telegram-chatbot/assets/161431602/f11b604f-652b-49ad-a51c-ffbba0d08780" width="70%" height="70%">
</p>

---

✅ 동작 순서:
- python script(telegramebot.py)를 실행하여 FastAPI 서버를 생성한다.
  - fastapi 단독으로는 웹개발을 할 수 없다. 따라서 비동기 서버를 생성하는 uvicorn을 추가로 설치한다.
  - pip install fastapi
  - pip install 'uvicorn[standard]'
    - p.s. FastAPI, Uvicorn으로 비동기 웹서버 띄우기: https://bit.ly/fastapi-and-uvicorn
- ngrok를 이용해서 '외부에서 로컬서버로 접속하기 위한 주소를 발급' 받는다. 
   - ngrok 사용방법(외부에서 Localhost 접속하는 방법): https://bit.ly/about-ngrok
- 발급받은 주소를 telegram api의 웹훅과 연결한다.
  - telegram api의 웹훅을 사용하여 텔레그램 서버와 로컬서버를 연결한다.    
<p align="center">
	<img alt="image" src="https://github.com/i-am-shuan/LLM-telegram-chatbot/assets/161431602/bda47a71-41a9-491e-84ea-5f39e709e9eb" width="70%" height="70%">
</p>

---

✅ service spec:
- fast api, ngrok, telegram api
- langchain, gpt-3.5-turbo, gpt-DALL.E 2

⚠️ 유의사항
- 실습을 진행하려면 PC나 개인 휴대전화에서 텔레그램을 설치하고, 회원가입 및 로그인이 완료된 상태여야 합니다.

---

🙋‍♂️ 따라하기
- telegram api 가이드: https://core.telegram.org
  - python tutorial bot: https://gitlab.com/Athamaxy/telegram-bot-tutorial/-/blob/main/TutorialBot.py
- 텔레그렘에서 'botfather'를 추가한다.
<p align="center">
	<img alt="image" src="https://github.com/i-am-shuan/LLM-telegram-chatbot/assets/161431602/94749745-b6af-42ea-a3dd-9ada15a897af" width="50%" height="50%">
</p>

- 새로운 챗봇을 생성한다: /newvot

<p align="center">
	<img alt="image" src="https://github.com/i-am-shuan/LLM-telegram-chatbot/assets/161431602/ec557766-8c62-48fb-8e8b-a93c305ef74e" width="50%" height="50%">
</p>

- 'bot'으로 끝나는 챗봇 입력하여 새로운 챗봇을 생성한다.
- 발급받은 access token 정보를 보관한다.

<p align="center">
	<img alt="image" src="https://github.com/i-am-shuan/LLM-telegram-chatbot/assets/161431602/e4266504-682a-48cd-af2a-cb77119b2ad3" width="50%" height="50%">
</p>

- 텔레그램 API URL 양식: https://api.telegram.org/bpt<token>/METHOD_NAME
  - 메세지 전송: https://api.telegram.org/bpt<token>/sendMessage
  - 사진 전송: https://api.telegram.org/bpt<token>/sendPhoto
- p.s. telegram bot tutorial: https://core.telegram.org/bots/tutorial

---

👀 결과
- GPT에게 질문하기
  - 명령어: /ask
<p align="center">
	<img alt="image" src="https://github.com/i-am-shuan/LLM-telegram-chatbot/assets/161431602/6ff6397a-cdfe-4690-9dbc-4d210a57f73e" width="50%" height="50%">
</p>

- DALL-E에게 이미지 작성 요청하기
  - 명령어: /img
<p align="center">
	<img alt="image" src="https://github.com/i-am-shuan/LLM-telegram-chatbot/assets/161431602/47388269-ae92-448d-a525-28ac6a7f70d9" width="50%" height="50%">
</p>

---
