## Getting started

Install non-standard packages:
```sh
pip install aiohttp, dotenv, twilio
```

Create a `.env` file by copying `env.example` and replacing placeholder values.

Get twilio to talk to your local dev instance by starting `ngrok`
```sh
ngrok http 8080
```
and having your twilio number POST to `<ngrok url>/twilio/twiml/start`.

Start the server:
```sh
python chat.py
```

Now, you can call your twilio number and talk to ChatGPT.
