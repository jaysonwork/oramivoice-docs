# Image Synthesis API

The Image Synthesis API allows developers to generate single images, run batch rendering queues, and retrieve generation history programmatically.

---

## 1. Generate Image Endpoint

**POST** `https://oramivoice.com/api/images/generate`

### Headers:
```http
Authorization: Bearer YOUR_API_KEY
Content-Type: application/json
```

### Request Parameters:

| Field | Type | Required | Default | Description |
| :--- | :--- | :--- | :--- | :--- |
| `prompt` | string | Yes | — | Text description of the desired image. |
| `model` | string | No | `GEM_PIX_2` | Model code: `GEM_PIX_2` (Nano Banana Pro) or `NARWHAL` (Nano Banana). |
| `aspect_ratio` | string | No | `IMAGE_ASPECT_RATIO_LANDSCAPE` | `IMAGE_ASPECT_RATIO_LANDSCAPE` (16:9), `IMAGE_ASPECT_RATIO_LANDSCAPE_FOUR_THREE` (4:3), `IMAGE_ASPECT_RATIO_SQUARE` (1:1), `IMAGE_ASPECT_RATIO_PORTRAIT_THREE_FOUR` (3:4), `IMAGE_ASPECT_RATIO_PORTRAIT` (9:16). |
| `image_urls` | array | No | `[]` | List of reference image URLs for style/subject conditioning (Img2Img). |

### Example Request (cURL):
```bash
curl -X POST "https://oramivoice.com/api/images/generate" \
  -H "Authorization: Bearer orami_live_xxxxxxxx" \
  -H "Content-Type: application/json" \
  -d '{
    "prompt": "Cinematic portrait of an astronaut on Mars at sunset, 8k resolution",
    "model": "GEM_PIX_2",
    "aspect_ratio": "IMAGE_ASPECT_RATIO_LANDSCAPE"
  }'
```

### Example Response:
```json
{
  "success": true,
  "data": {
    "task_id": "nanoai_34746b9d",
    "image_url": "https://oramivoice.com/storage/images/nanoai_34746b9d.jpg",
    "model": "GEM_PIX_2",
    "ratio": "IMAGE_ASPECT_RATIO_LANDSCAPE",
    "duration": 4.25,
    "credits_used": 2000,
    "user_credits": {
      "remaining": 48451211
    }
  }
}
```

---

## 2. Image Generation History Endpoint

**GET** `https://oramivoice.com/api/images/history?limit=30`

### Headers:
```http
Authorization: Bearer YOUR_API_KEY
```

### Response:
```json
{
  "success": true,
  "data": {
    "images": [
      {
        "id": 142,
        "task_id": "nanoai_34746b9d",
        "prompt": "Cinematic portrait of an astronaut on Mars",
        "model": "GEM_PIX_2",
        "aspect_ratio": "IMAGE_ASPECT_RATIO_LANDSCAPE",
        "image_url": "https://oramivoice.com/storage/images/nanoai_34746b9d.jpg",
        "created_at": "2026-09-28 00:39:27"
      }
    ]
  }
}
```
