1. Make sure your docker engine is ruuning
2. Place your .env file in every service folder. the file contents should be the following ->> OPENAI_API_KEY='$YOUR_OPENAI_API_KEY'
3. Open CMD and CD into the app folder
4. run the following command --->> docker-compose build up -d
5. After completion, open http://localhost:8501 in the browser
