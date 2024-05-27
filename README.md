# Gemini Dynamo
The GeminiDynamo project integrates frontend and backend technologies to efficiently parse and organize lengthy YouTube transcripts, revolutionizing study processes and enhancing digital learning experiences. 

The project uses DynamoCards, an open-source tool, tackles the arduous task of parsing lengthy YouTube transcripts with its Semantic Extraction Algorithm (SEA), aiming to streamline the study process for students and educators. By swiftly identifying and organizing key concepts and terms within university lectures and other lengthy video content, DynamoCards revolutionizes digital learning, facilitating more effective study habits and enhancing classroom instruction. It empowers users to distill hours of lecture material into concise, digestible insights, marking a significant advancement in educational technology.

## Installation

1. Enable Google Cloud through this [Link](https://cloud.google.com/cloud-console?utm_source=google&utm_medium=cpc&utm_campaign=na-US-all-en-dr-bkws-all-all-trial-e-dr-1707554&utm_content=text-ad-none-any-DEV_c-CRE_665735422256-ADGP_Hybrid%20%7C%20BKWS%20-%20MIX%20%7C%20Txt-Management%20Tools-Cloud%20Console-KWID_43700077225654741-kwd-55675752867&utm_term=KW_google%20cloud%20console-ST_google%20cloud%20console&gad_source=1&gclid=Cj0KCQiArrCvBhCNARIsAOkAGcXO2_affz2IH9q_ps1LDwrdsOe43AmOiJps1j9UK_ri0mnBWRd9eA0aApkNEALw_wcB&gclsrc=aw.ds).
- Go to vertexAI and 'Enable All Recommended APIs'
- Go to 'IAM & Admin' and then 'Service Accounts'
- Create a service account and download the .json file.
- Run the following command in VSCode
  ```
  export GOOGLE_APPLICATION_CREDENTIALS = "/path/to/your/authentication-file.json"
  ```

2. Open VSCode and enter the following text:
   ```
   gcloud init
   ```

3. Create new or re-initialize your configuration, log in with your account, and create or choose your project.
   ![image](https://github.com/philliphjhuang/RadicalX/assets/30792325/6e345325-36fb-4ba8-b65a-82d2cb023294)

4. Install the packages in requirement.txt in the backend directory:
   ```
   cd backend
   pip install -r requirements.txt
   ```
   
5. In the terminal, run the following command for the backend:
   ```
   cd backend
   uvicorn main:app --reload
   ```
   
6. Create a new terminal without closing the previous one and run the following commands for the frontend:
   ```
   cd frontend/dynamocards
   npm run dev
   ```
   
7. In your browser, open the following links:
   [backend](http://127.0.0.1:8000/docs)
   [frontend](http://localhost:5173/)

8. Navigate through the following in the **backend** link:
   - ![Screenshot](https://github.com/philliphjhuang/GeminiDynamo/assets/30792325/db3f5e52-9cdc-48d7-a262-1f458ee88604)
   - ![Screenshot](https://github.com/philliphjhuang/GeminiDynamo/assets/30792325/8657e37b-bc1f-4adb-bd90-0d62d84ecdc7)
   - ![Screenshot](https://github.com/philliphjhuang/GeminiDynamo/assets/30792325/4ba12f12-1441-45b8-aa6c-b1df5ea33d84)
     - replace https://example.com/ with any YouTube link of your choice (Preferably videos with captions)
   - Click on the "Execute" button.
   - If successful, it will show Code 200 like in the following screenshot:
     - ![Screenshot](https://github.com/philliphjhuang/GeminiDynamo/assets/30792325/985dcb5f-eccb-4ecc-a289-e5c634fc8791)
   - If not successful, it will show Code 500. Try executing again or with a different YouTube link.

9. Navigate through the following in the **frontend** link:
   - ![image](https://github.com/philliphjhuang/GeminiDynamo/assets/30792325/3a0050cf-4e47-45db-960d-233e1c34aa83)
     - Enter the same YouTube that you entered for backend and click on "Generate Flashcards"

10. Results:
    ![image](https://github.com/philliphjhuang/GeminiDynamo/assets/30792325/306f6118-832c-403e-828a-0da8371dbc68)



   
   


## Functions
Allows users to upload multiple PDFs, enter a topic, choose the number of questions, and generate a multiple-choice quiz based on the PDFs and the topic.
![image](https://github.com/philliphjhuang/GeminiQuizify/assets/30792325/001ddd74-2e66-44bd-b98b-a87cda062d0d)

After pressing submit, it generates question(s) and allows to user to choose answer choices, submit, and go to next/previous questions.

![image](https://github.com/philliphjhuang/GeminiQuizify/assets/30792325/a4b8602e-81e1-455c-b19a-e139f2be3055)

# Video demonstration
[Watch the video](https://www.loom.com/share/e36fc7013b0b4a138ffb630db3ed7cfe?sid=2d31deb6-960b-4b7a-ac35-c082e96ea4ae)

# Certificate
![image](https://github.com/philliphjhuang/GeminiQuizify/assets/30792325/12c1c88c-9ef9-47e6-ab77-0b5e207bfb9c)

## Contributers
- Phillip Huang
  - [Linkedin](https://www.linkedin.com/in/phillip-huang-449b64229/)
  - [Github](https://github.com/philliphjhuang)
- Radical AI for providing this experience on AI Engineering.
