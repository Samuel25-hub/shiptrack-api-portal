# POST /shipments

Create a new shipment record.

---

## Endpoint

```text
POST /shipments
```

---

## Request Headers

| Header | Value |
|---|---|
| Authorization | Bearer YOUR_API_KEY |
| Content-Type | application/json |

---

## Example Request Body

```json
{
  "origin": "Houston, TX",
  "destination": "Dallas, TX",
  "package_weight": 12,
  "delivery_type": "Express"
}
```

---

## Example Request

```bash
curl -X POST https://api.shiptrack.com/v1/shipments \
-H "Authorization: Bearer YOUR_API_KEY" \
-H "Content-Type: application/json"
```

---

## Example Response

```json
{
  "shipment_id": "ST-1050",
  "status": "Pending",
  "message": "Shipment created successfully"
}
```

---

## Status Codes

| Code | Meaning |
|---|---|
| 201 | Shipment Created |
| 400 | Invalid Request |
| 401 | Unauthorized |
| 500 | Internal Server Error |
