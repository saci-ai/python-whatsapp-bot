# Using Heroku to deploy the APP

Replace `<heroku-app>` by the app name you created on Heroku 

```
# tagging your image to heroku registry
docker tag python-whatsapp-bot:latest registry.heroku.com/<heroku-app>/web

# pushing your image to heroku registry
docker push registry.heroku.com/<heroku-app>/web

# releasing your container
heroku container:release web --app <heroku-app>

# checking logs
heroku logs --app <heroku-app> --tail

# restarting your app
heroku ps:restart --app <heroku-app>

# executing the bash of your container
heroku run bash --app <heroku-app>
```
