# Error Handling

ShipTrack API uses standard HTTP status codes to indicate request success or failure.

---

## Common Error Codes

| Status Code | Meaning |
|---|---|
| 400 | Bad Request |
| 401 | Unauthorized |
| 404 | Resource Not Found |
| 500 | Internal Server Error |

---

## Example Error Response

```json
{
  "error": "Unauthorized",
  "message": "Invalid API token"
}
```
