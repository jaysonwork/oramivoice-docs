# Speech Synthesis API

The Speech Synthesis API enables programmatic text-to-speech generation via REST HTTP requests.

---

## Endpoint Specification

**POST** `https://oramivoice.com/api/v1/tts/generate`

### Headers:
```http
Authorization: Bearer YOUR_API_KEY
Content-Type: application/json
```

### Request Body Parameters:

| Parameter | Type | Required | Default | Description |
| :--- | :--- | :--- | :--- | :--- |
| `text` | string | Yes | — | The text or script content to synthesize. |
| `voice_id` | string | Yes | — | ID of the target voice model from the Voice Library. |
| `speed` | float | No | `1.0` | Speech rate multiplier between `0.5` and `2.0`. |
| `pitch` | float | No | `0.0` | Vocal pitch offset between `-50.0` and `+50.0`. |
| `format` | string | No | `mp3` | Audio format: `mp3` or `wav`. |

---

## Code Examples

### cURL
```bash
curl -X POST "https://oramivoice.com/api/v1/tts/generate" \
  -H "Authorization: Bearer orami_live_xxxxxxxx" \
  -H "Content-Type: application/json" \
  -d '{
    "text": "Welcome to OramiVoice AI Speech Synthesis.",
    "voice_id": "voice_en_narrator_01",
    "speed": 1.0,
    "format": "mp3"
  }'
```

### Python
```python
import requests

url = "https://oramivoice.com/api/v1/tts/generate"
headers = {
    "Authorization": "Bearer orami_live_xxxxxxxx",
    "Content-Type": "application/json"
}
payload = {
    "text": "Welcome to OramiVoice AI Speech Synthesis.",
    "voice_id": "voice_en_narrator_01",
    "speed": 1.0,
    "format": "mp3"
}

response = requests.post(url, json=payload, headers=headers)
data = response.json()

if data.get("success"):
    print("Audio URL:", data["data"]["audio_url"])
    print("Duration:", data["data"]["duration_seconds"])
```
