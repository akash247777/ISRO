# ISRO

<img width="1600" height="900" alt="WhatsApp Image 2026-10-26 at 8 16 53 PM" src="https://github.com/user-attachments/assets/6c751332-8b75-4e85-b3f8-14b065794d2a" />
<img width="1600" height="900" alt="WhatsApp Image 2026-10-26 at 8 16 52 PM (1)" src="https://github.com/user-attachments/assets/0a61bac6-ad7a-4566-b28c-62e6de0dae9b" />
<img width="1600" height="900" alt="WhatsApp Image 2026-10-26 at 8 16 52 PM" src="https://github.com/user-attachments/assets/4782abd3-7233-48f7-a8fc-0991a4d8fda6" />




curl "https://generativelanguage.googleapis.com/v1beta/openai/chat/completions" \
-H "Authorization: Bearer AIzaSyDtxPMEsk6qaN0c0dTb25hbNQcKLpqoS" \
-H "Content-Type: application/json" \
-d '{
  "model": "gemini-2.5-flash-lite",
  "messages": [
    {
      "role": "system",
      "content": "help for interview"
    },
    {
      "role": "user",
      "content": [
        {
          "type": "text",
          "text": "{{TEXT}}"
        },
        {
          "type": "image_url",
          "image_url": {
            "url": "data:image/png;base64,{{IMAGE}}"
          }
        }
      ]
    }
  ]
}'


choices[0].message.content
