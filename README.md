# ChatGPT를 이용한 PC 부품 추천 & PC 질문 서비스
  * 예산과 용도, 요구사항 등을 입력하면 chatGPT를 통해서 적절한 PC 부품을 추천해주는 웹 서비스 입니다.
  * 컴퓨터의 하드웨어 종류와 추천해주는 부품에 대한 정보를 챗봇에게 물어볼 수 있습니다.
  * 내 PC가 고장나거나 어떠한 문제가 있을 때 챗봇에게 물어볼 수 있습니다.
## 1. 목표와 기능
  1.1 목표

  * 컴퓨터에 대해서 관심 없거나 잘 모르는 사람들에게 유용한 정보를 제공하는 서비스
  * PC 구매부터 이후 사용시 일어나는 문제까지 모든 도움을 받을 수 있는 서비스
  * 컴퓨터에 대한 지식이 부족해서 일어날수있는 안타까운 문제와 상황을 방지하는 서비스

1.2 기능

  * ChatGPT를 활용해서 예산과 용도에 따라 적절한 견적을 추천
  * ChatGPT를 활용해서 부족한 컴퓨터 지식을 챗봇에게 물어볼 수 있음
## 2. 개발 환경 및 배포 URL
  2.1 개발 환경
  * Web 구현
     * JavaScript
  * 서비스 배포
     * Github Page
   
  2.2 배포 URL
  
  https://userdonghu.github.io/chatGPT_Project/
  

## 3. 프로젝트 파일 설명 및 구현 기능
  3.1 프로젝트 파일 설명
  
   <img width="173" alt="image" src="https://github.com/UserDongHu/chatGPT_Project/assets/137512514/a20652d2-8c93-4039-8cc0-3eb44917930a">

   - index.html
     - 초기화면을 보여준다
   - pcGPT.js
     - 초기 화면에서 PC견적, PC질문을 각각 클릭했을 때의 화면을 변경하고, 로고를 누르면 다시 초기 화면을 보여준다.
     - PC견적 화면을 선택했을 때, ChatGPT API를 이용하여 폼에 입력받은 값을 데이터로 넘기고, 결과를 출력한다.
     - 출력된 PC견적 결과를 로컬스토리지에 저장하고, 로컬스토리지에 저장된 값을 불러와서 출력한다.
     - PC질문 화면을 선택했을 때, ChatGPT API를 이용하여 입력받은 질문을 데이터로 넘기고, 그 결과를 채팅형식으로 출력한다.
   - recommend.js
     - PC견적 화면을 선택했을 때, 사용자가 입력할 폼을 만든다.
     - 폼에 입력받은 값을 분류하여 배열로 정리하고, 이를 하이퍼링크로 생성하여 반환한다.
   - question.js
     - PC선택 화면을 선택했을 때, 질문을 입력할 폼을 만든다.
     - 질문과 답변을 구분한다.
    
  3.2 구현 기능

   - 메인화면
     - 
   - PC견적
   - PC질문

## 4. 역할 분담

  * 개인 프로젝트

## 5. UI / BM
  ![메인화면](https://github.com/UserDongHu/chatGPT_Project/assets/137512514/10f07725-7b2a-41a5-b814-6c9cf48f88dc)
  메인화면에서 PC견적과 PC질문을 선택할 수 있으며, 로고를 클릭시 다시 메인 화면이 나타난다. <br><br>

  ![PC견적2](https://github.com/UserDongHu/chatGPT_Project/assets/137512514/6887ff07-0f8c-4583-84fd-2515ae75b5bd)
  PC견적 화면에서 사용자가 폼에 입력하고 견적 추천 버튼을 누르면 잠시만 기다려주세요 문구가 나온 후, chatGPT가 추천해준 적절한 견적을 보여준다.<br><br>

  ![PC견적3](https://github.com/UserDongHu/chatGPT_Project/assets/137512514/9d2f0e68-c502-40ee-9751-111afcc574a1)
  견적 저장을 누르면 로컬 스토리지에 견적이 저장되며 저장된 견적 보기를 누르면 저장된 견적을 보여주고, 견적 삭제를 누르면 저장된 견적이 삭제된다.<br><br>

  ![PC견적4](https://github.com/UserDongHu/chatGPT_Project/assets/137512514/eb649f2a-c007-4ebd-83bd-6c7db749d17e)
  견적 추천 버튼 혹은 저장된 견적 보기 버튼을 통해 나타난 견적의 부품을 클릭하면 이를 구매할 수 있는 쇼핑몰 사이트로 이동한다.<br><br>

  ![PC질문1](https://github.com/UserDongHu/chatGPT_Project/assets/137512514/3f253cce-e943-4187-bf06-1dcc3f9c2cfd)
  PC질문 화면에서 컴퓨터에 대한 다양한 질문을 할 수 있으며, 잠시만 기다려주세요 문구가 나온 후, 내 질문과 chatGPT의 답변이 채팅 형식으로 표시된다.<br><br>

  ![PC질문2](https://github.com/UserDongHu/chatGPT_Project/assets/137512514/81505fd6-9522-4001-a88a-0c0283aa328b)
  질문을 했지만 조금 더 궁금한 것이 있거나 더 질문할 것이 남아있을 경우, 추가로 질문을 하면 chatGPT가 이어서 답변을 해준다.


## 6. 개발하며 느낀점
