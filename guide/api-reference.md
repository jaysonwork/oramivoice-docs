# Developer API Reference

Integrate OramiVoice generative AI capabilities directly into your applications, bots, and backend pipelines.

---

## 🔑 Authentication

All API requests require your Secret API Key passed in the `Authorization` or `x-api-key` header:

```http
Authorization: Bearer orami_live_xxxxxxxxxxxxxxxx
Content-Type: application/json
```

Generate your API key from the **API Keys** section in your [Profile](https://oramivoice.com/api-keys.php).

---

## 🎨 Image Generation Endpoint

**POST** `https://oramivoice.com/api/images/generate`

### Request Body:
```json
{
  "prompt": "A majestic golden retriever sitting in a field of sunflowers, 4k",
  "model": "GEM_PIX_2",
  "aspect_ratio": "IMAGE_ASPECT_RATIO_LANDSCAPE"
}
```

### Models:
- `GEM_PIX_2` (Nano Banana Pro): 2,000 credits
- `NARWHAL` (Nano Banana): 1,500 credits

### Response:
```json
{
  "success": true,
  "data": {
    "task_id": "nanoai_xxxx",
    "image_url": "https://oramivoice.com/storage/images/nanoai_xxxx.jpg",
    "model": "GEM_PIX_2",
    "credits_used": 2000,
    "user_credits": {
      "remaining": 48451211
    }
  }
}
```
