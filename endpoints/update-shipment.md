# PUT /shipments/{id}

Update the status of an existing shipment.

---

## Endpoint

```text
PUT /shipments/{id}
```

---

## Path Parameters

| Parameter | Type | Description |
|---|---|---|
| id | string | Unique shipment identifier |

---

## Example Request Body

```json
{
  "status": "Delivered"
}
```

---

## Example Request

```bash
curl -X PUT https://api.shiptrack.com/v1/shipments/ST-1001 \
-H "Authorization: Bearer YOUR_API_KEY" \
-H "Content-Type: application/json"
```

---

## Example Response

```json
{
  "shipment_id": "ST-1001",
  "status": "Delivered",
  "message": "Shipment updated successfully"
}
```

---

## Status Codes

| Code | Meaning |
|---|---|
| 200 | Shipment Updated |
| 400 | Invalid Request |
| 401 | Unauthorized |
| 404 | Shipment Not Found |
