# Bolo--WhatsApp-
from flask import Flask, request app = Flask(__name__)  @app.route("/webhook", methods=["POST"]) def webhook():     message = request.json["data"]["message"]["conversation"]     # ici tu appelles TA fonction IA déjà codée     reponse = ton_ia(message)     return {"reply": reponse}
