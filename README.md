# AI Voice Receptionist – Dental Clinics (Mumbai)

Built using n8n + OpenAI + Telegram + Google Calendar.

This project is a fully automated Voice AI Receptionist created for a four-clinic dental brand in Mumbai.  
Users send voice messages on Telegram; the AI understands treatment queries, books appointments, replies back in voice and text, and sends email confirmations.  
Built entirely using AI tools for the Purple Focus AI Labs assignment.

---

## Demo Video
(Upload demo.mp4 to this repo and paste the link here.)

---

## Screenshots

[Screenshot (319).png](https://github.com/vinithabhj/voice-ai-receptionist-dental-mumbai/blob/2c501e984866cb724e4b12797081497c2bcaa4d7/Screenshot%20(319).png)

Screenshot (320).png

WhatsApp Image 2025-11-06 at 13.26.45_b36b3baa.jpg

WhatsApp Image 2025-11-06 at 13.31.43_068f8d88.jpg

---

## Features
- Voice → AI → Voice receptionist  
- Transcribes user speech using Whisper  
- Answers dental treatment queries  
- Books appointments with follow-up questions  
- Google Calendar integration  
- Multi-clinic routing (Bandra / Andheri / Ghatkopar / Thane)  
- Sends confirmation via Telegram (text + voice)  
- Email confirmation with precautions  
- Cancel and reschedule support  
- Built fully using n8n and OpenAI

---

## Workflow Summary
1. User sends a voice message on Telegram  
2. n8n downloads the audio and transcribes it using Whisper  
3. GPT-4o extracts intent and required fields (clinic, date, time, treatment)  
4. If booking:
   - Resolves date/time in IST  
   - Routes clinic to correct Google Calendar  
   - Creates the event  
5. AI replies back via voice (OpenAI TTS), text (Telegram), and email (Gmail OAuth)  
6. For treatment questions, the AI gives safe, friendly answers  
7. For cancellations/rescheduling, it updates or deletes the event  

---

## Tech Stack
| Component | Tool |
|----------|------|
| Automation | n8n |
| Speech-to-Text | OpenAI Whisper |
| Reasoning | GPT-4o |
| Text-to-Speech | OpenAI TTS |
| Calendar | Google Calendar API |
| Messaging | Telegram Bot |
| Email | Gmail OAuth |

---

## How to Run
1. Clone or download this repository  
2. Import the .json workflow file into n8n  
3. Add credentials:
   - OpenAI API Key  
   - Telegram Bot Token  
   - Google Calendar OAuth  
   - Gmail OAuth  
4. Start the Telegram bot and send a voice message  
5. The bot responds with voice and text and manages appointments end-to-end

---

## One-Page Summary
This Voice AI Receptionist demonstrates:
- Real conversational AI  
- Multi-tool automation (n8n + OpenAI + Telegram + Google Calendar)  
- A production-ready workflow  

---

## Author
**Vinitha Kurapati**  
AI Automations • OpenAI Integrations • Voice AI Systems

