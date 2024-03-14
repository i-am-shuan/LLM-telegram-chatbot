# LLM-telegram-chatbot
- ChatGPT로 질의응답 및 DALLE.2 모델기반 그림을 그려주는 AI 챗봇
<p align="center">
	<img alt="image" src="https://github.com/i-am-shuan/LLM-telegram-chatbot/assets/161431602/f11b604f-652b-49ad-a51c-ffbba0d08780" width="70%" height="70%">
</p>

✅ service spec:
- fast api, ngrok, telegram api
- langchain, gpt-3.5-turbo, gpt-DALL.E 2

⚠️ 유의사항
- 실습을 진행하려면 PC나 개인 휴대전화에서 텔레그램을 설치하고, 회원가입 및 로그인이 완료된 상태여야 합니다.

🙋‍♂️ 따라하기
- telegram api 가이드: https://core.telegram.org
  - python tutorial bot: https://gitlab.com/Athamaxy/telegram-bot-tutorial/-/blob/main/TutorialBot.py
- ngrok 사용방법(외부에서 Localhost 접속하는 방법)
  - https://velog.io/@kya754/ngrok-%EC%82%AC%EC%9A%A9%ED%95%98%EA%B8%B0
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
- 텔레그램 API URL 양식
<p align="center">
	<img alt="image" src="https://github.com/i-am-shuan/LLM-telegram-chatbot/assets/161431602/af602737-36b6-428e-a2e4-a03b2792e268" width="50%" height="50%">
</p>
- 상세 정보는 튜토리얼을 참고한다: https://core.telegram.org/bots/tutorial

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
