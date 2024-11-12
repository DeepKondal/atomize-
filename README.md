(If running locally)
1. Make sure your docker engine is ruuning
2. Place your .env file in every service folder. the file contents should be the following ->> OPENAI_API_KEY='$YOUR_OPENAI_API_KEY'
3. remove comment on loadenv in each service file's app.py
4. remove comment on this part :
    #env_file:
    #  - ./introduction_service/.env
   for every service in the docker-compose.yml file
5. remove comment on this part:
    #COPY .env /app/.env
    on every Dockerfile in every service
6. Open CMD and CD into the app folder
7. run the following command --->> docker-compose build up -d
8. After completion, open http://localhost:8501 in the browser

(If running on VM/Cloud)
Since all the environment variables and secrets are on github, it should work as it is with the following command -->>> <<docker-compose -p atomize up --build -d>>
and the CI/CD established
