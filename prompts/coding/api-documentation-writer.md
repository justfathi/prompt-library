---
title: API Documentation Writer
industry: coding
tags: [documentation, api, developer-experience, openapi, reference]
contributor: justfathi
---

## Description
Generates clear, structured API reference documentation from a function signature, route definition, or code — including parameters, response schemas, error codes, and usage examples.

## Use Case
Backend developers and developer experience teams who need to document an API endpoint or SDK method without spending time manually writing reference docs.

## The Prompt
```
You are a technical writer specializing in developer documentation. Generate complete API reference documentation for the endpoint or function below.

Use this structure:

---

## [Method] `[ENDPOINT PATH or FUNCTION NAME]`

**Description**
[1–2 sentences explaining what this endpoint/function does and when to use it]

**Authentication**
[Required / Optional / None — and what type: Bearer token, API key, OAuth, etc.]

---

### Request

**Method:** `[GET / POST / PUT / PATCH / DELETE]`
**URL:** `[FULL PATH]`

**Path Parameters**
| Parameter | Type | Required | Description |
|-----------|------|----------|-------------|
| [param] | string | Yes | [what it is] |

**Query Parameters**
| Parameter | Type | Required | Default | Description |
|-----------|------|----------|---------|-------------|
| [param] | string | No | null | [what it does] |

**Request Body** (if applicable)
Content-Type: `application/json`
```json
{
  "field": "type — description"
}
```

**Field descriptions:**
| Field | Type | Required | Description |
|-------|------|----------|-------------|

---

### Response

**Success Response: `200 OK`** (or relevant code)
```json
{
  "example": "response"
}
```

**Response Fields:**
| Field | Type | Description |
|-------|------|-------------|

---

### Error Responses

| Status Code | Error Code | Description | Resolution |
|-------------|------------|-------------|------------|
| 400 | INVALID_REQUEST | [reason] | [how to fix] |
| 401 | UNAUTHORIZED | [reason] | [how to fix] |
| 404 | NOT_FOUND | [reason] | [how to fix] |
| 500 | SERVER_ERROR | [reason] | [how to fix] |

---

### Code Examples

**cURL**
```bash
curl -X [METHOD] "[URL]" \
  -H "Authorization: Bearer YOUR_TOKEN" \
  -H "Content-Type: application/json" \
  -d '{"field": "value"}'
```

**JavaScript (fetch)**
```javascript
// example
```

**Python**
```python
# example
```

---

### Notes
[Any rate limits, pagination details, side effects, or gotchas worth calling out]

---

Endpoint or function to document:
```[LANGUAGE]
[PASTE THE ROUTE DEFINITION, FUNCTION SIGNATURE, OR CODE HERE]
```

Additional context:
- What does this endpoint/function do? [PLAIN ENGLISH]
- Authentication scheme: [AUTH TYPE]
- Any known edge cases or limits: [RATE LIMITS, MAX SIZE, ETC.]
```

## Notes
- For REST APIs, paste the route handler — the model will infer path params, query params, and request body from the code
- For SDK methods, paste the function signature and any inline comments
- Generated error code tables should be verified against the actual implementation
- Pair with an OpenAPI spec generation prompt to produce machine-readable docs
