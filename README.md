## Laravel API Token Auth with Next.js Frontend

Laravel Breeze is an implementation of all of Laravel&apos;s authentication features, including login, registration, password reset, email verification, and password confirmation.
Breeze includes a simple &quot;profile&quot; page where the user may update their name, email address, and password.

Laravel Breeze&apos;s default view layer comprises simple Blade templates styled with Tailwind CSS. Or, Breeze can scaffold the application using Vue or React and Inertia.
Laravel Breeze can also scaffold an authentication API ready to authenticate modern JavaScript applications such as Next, and others.

This project is trying to <b>use Laravel Breeze API as the backend and set up authentication with Next.js as the browser frontend</b>. Laravel Sanctum is incorporated with Laravel Breeze to provide the authentication system.
Sanctum is a simple package you can use to issue API tokens to your users without the complication of OAuth. 
When making requests using API tokens, the token should be included in the Authorization header as a Bearer token. The Next.js React front pages are styled with Tailwind CSS to follow Laravel Breeze&apos;s default view designs. 

### Docker:
```
# Run the following two commands simutaneously with diffrent screen windows...

docker run -it -p 8000:8000 jglchen/user-api-token php artisan serve --host=0.0.0.0
docker run -p 3000:3000 jglchen/user-next-token
```

### Docker Compose:
```
# At the root of the /user-laravel-next folder...
docker compose up
```
