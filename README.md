# AWS Language Translator Bot

A serverless chatbot built with **AWS Lex V2**, **Lambda**, and **Amazon Translate** to translate user input into multiple languages.

## Demo Video
Watch it in action:

![Demo Video](demo-video.mp4)

Or download [here](demo-video.mp4)

---

## Tech Stack
- **Amazon Lex V2** – Bot interface, intents, and slot management
- **AWS Lambda** – Fulfillment logic (Python)
- **Amazon Translate** – Translation API
- **Amazon Comprehend** – Source language detection
- **AWS CLI** – Bot deployment and management

---

## Features
- Multi-language translation
- Automatic source language detection
- Dynamic slot handling in Lex
- Serverless architecture

---

## Example Prompts
| Input Text | Target Language | Bot Response |
|------------|----------------|--------------|
| hello      | Spanish        | hola         |
| thanks     | French         | merci        |
| peace      | Japanese       | 平和 (heiwa) |

---

## Usage
1. Deploy Lambda function (`lambda_function.py`) in AWS Lambda.  
2. Configure Lex V2 bot with `TranslateIntent` and `FallbackIntent`.  
3. Connect Lambda function to Lex as the fulfillment code hook.  
4. Test in Lex Test Bot or via Web UI.

---

## Optional Extensions
- Add more languages & synonyms in `LANG_MAP`
- Add a `SourceLanguage` slot for user-specified source language
- Embed via Lex Web SDK for a live interactive demo
