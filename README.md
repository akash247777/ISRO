# ISRO




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
