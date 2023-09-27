# Voxa Web Translation API

Welcome to the Voxa Translation API! Easily translate text between different languages using a simple HTTP request.

## Table of Contents

- [Endpoint](#endpoint)
- [Parameters](#parameters)
- [Response Format](#response-format)
- [Example](#example)
- [Support & Feedback](#support--feedback)

## Endpoint

```
https://voxa.dark9015.repl.co/api
```

## Parameters

| Parameter   | Description                                                   | Example |
|-------------|---------------------------------------------------------------|---------|
| `translate` | The text you wish to translate.                               | Hello   |
| `from`      | The original language of the text (ISO 639-1 code).           | en      |
| `to`        | The target language to which you want the text translated (ISO 639-1 code). | fr |

**Note**: Ensure all parameters are URL encoded to handle special characters and spaces.

## Response Format

The API returns a JSON object containing the following fields:

| Field       | Description                                |
|-------------|--------------------------------------------|
| `translated`| The translated text.                       |
| `original`  | The original text that was to be translated|
| `from`      | The original language of the text.         |
| `to`        | The language to which the text was translated. |

## Example

**Request**:
```
https://voxa.dark9015.repl.co/api?translate=Hello&from=en&to=fr
```

**Response**:
```json
{
    "translated": "Bonjour",
    "original": "Hello",
    "from": "en",
    "to": "fr"
}
```

Happy Translating! 🌍