## How to start project:

1. Clone this repository

2. Run `composer install`

3. Copy `.env.example` to `.env`

4. Add your OpenAI API key in `.env` file at `OPENAI_API_KEY`

5. Add your SMTP configuration. This will be used to send your conversation to your email.

6. Run `php artisan key:generate`

7. Run `php artisan migrate`

8. Run `php artisan storage:link`

9. Run `npm install`

10. Run `npm run build`

11. Run `php artisan serve`

12. Add the following line to your cronjobs:

`* * * * * cd /path-to-your-project && php artisan schedule:run >> /dev/null 2>&1`

The above will be used for the email queue job that it is used for sending the emails

13. Open the link: http://127.0.0.1:8000

## How to use

1. Start a conversation with the chatbot on the dashboard page.

2. When you finish the conversation, you can save it or send it to your email.

3. You can view your saved conversations on the dashboard page using pagination.

4. You can upload an audio file and ChatGPT will create the transcription for you.

5. You can also use `php artisan chat` command in order to ask ChatGPT from CLI.
