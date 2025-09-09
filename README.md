# json 
{
  "name": "m1_estetica",
  "language": "es",
  "category": "MARKETING",
  "components": [
    {
      "type": "BODY",
      "text": "Hola {{1}}, en 14 días activamos 10–20 valoraciones de {{2}} sin anuncios. ¿Te va una llamada de 8 min? Agenda aquí: {{3}}"
    },
    {
      "type": "FOOTER",
      "text": "Responde STOP para dejar de recibir mensajes."
    },
    {
      "type": "BUTTONS",
      "buttons": [
        {
          "type": "URL",
          "text": "Abrir agenda",
          "url": "https://calendly.com/chrisribera28/30min"
        }
      ]
    }
  ]
}
{
  "name": "m1_generico",
  "language": "es",
  "category": "MARKETING",
  "components": [
    {
      "type": "BODY",
      "text": "Hola {{1}}, en 14 días activamos 10–20 citas calificadas sin anuncios. ¿Te va una llamada de 8 min? Agenda aquí: {{2}}"
    },
    {
      "type": "FOOTER",
      "text": "Responde STOP para dejar de recibir mensajes."
    },
    {
      "type": "BUTTONS",
      "buttons": [
        {
          "type": "URL",
          "text": "Abrir agenda",
          "url": "https://calendly.com/chrisribera28/30min"
        }
      ]
    }
  ]
}
{
  "name": "m1_talleres",
  "language": "es",
  "category": "MARKETING",
  "components": [
    {
      "type": "BODY",
      "text": "Hola {{1}}, vi un detalle de tu taller. En 14 días activamos 10–20 citas sin anuncios. ¿Te va una llamada de 8 min? Agenda aquí: {{2}}"
    },
    {
      "type": "FOOTER",
      "text": "Responde STOP para dejar de recibir mensajes."
    },
    {
      "type": "BUTTONS",
      "buttons": [
        {
          "type": "URL",
          "text": "Abrir agenda",
          "url": "https://calendly.com/chrisribera28/30min"
        }
      ]
    }
  ]
}
{
  "name": "m2_recordatorio",
  "language": "es",
  "category": "UTILITY",
  "components": [
    {
      "type": "BODY",
      "text": "Hola {{1}}, ¿te reservo 8 min? Mi agenda: {{2}}. Si lo prefieres, dime 2 horarios por WhatsApp."
    },
    {
      "type": "FOOTER",
      "text": "Gracias por tu tiempo."
    },
    {
      "type": "BUTTONS",
      "buttons": [
        {
          "type": "URL",
          "text": "Abrir agenda",
          "url": "https://calendly.com/chrisribera28/30min"
        }
      ]
    }
  ]
}
{
  "name": "noshow_reprog",
  "language": "es",
  "category": "UTILITY",
  "components": [
    {
      "type": "BODY",
      "text": "¿Todo bien, {{1}}? Reprograma aquí: {{2}}. Puedo llamarte a {{3}} o {{4}}."
    },
    {
      "type": "FOOTER",
      "text": "Te tardará menos de 1 minuto."
    },
    {
      "type": "BUTTONS",
      "buttons": [
        {
          "type": "URL",
          "text": "Reprogramar",
          "url": "https://calendly.com/chrisribera28/30min"
        }
      ]
    }
  ]
}
{
  "info": {
    "name": "WhatsApp Cloud API — Chris (Templates + Send, full set)",
    "_postman_id": "1f3cf1d2-5c42-4f1d-9f2b-fullset",
    "description": "Crea 5 plantillas (3 marketing + 2 utility) y pruebas de envío.",
    "schema": "https://schema.getpostman.com/json/collection/v2.1.0/collection.json"
  },
  "item": [
    {
      "name": "Create Template — m1_talleres (MARKETING)",
      "request": {
        "method": "POST",
        "header": [
          {
            "key": "Authorization",
            "value": "Bearer {{ACCESS_TOKEN}}"
          },
          {
            "key": "Content-Type",
            "value": "application/json"
          }
        ],
        "url": {
          "raw": "https://graph.facebook.com/v19.0/{{WABA_ID}}/message_templates",
          "protocol": "https",
          "host": [
            "graph",
            "facebook",
            "com"
          ],
          "path": [
            "v19.0",
            "{{WABA_ID}}",
            "message_templates"
          ]
        },
        "body": {
          "mode": "raw",
          "raw": "{\n  \"name\": \"m1_talleres\",\n  \"language\": \"es\",\n  \"category\": \"MARKETING\",\n  \"components\": [\n    {\n      \"type\": \"BODY\",\n      \"text\": \"Hola {{1}}, vi un detalle de tu taller. En 14 días activamos 10–20 citas sin anuncios. ¿Te va una llamada de 8 min? Agenda aquí: {{2}}\"\n    },\n    {\n      \"type\": \"FOOTER\",\n      \"text\": \"Responde STOP para dejar de recibir mensajes.\"\n    },\n    {\n      \"type\": \"BUTTONS\",\n      \"buttons\": [\n        {\n          \"type\": \"URL\",\n          \"text\": \"Abrir agenda\",\n          \"url\": \"https://calendly.com/chrisribera28/30min\"\n        }\n      ]\n    }\n  ]\n}"
        }
      }
    },
    {
      "name": "Create Template — m1_estetica (MARKETING)",
      "request": {
        "method": "POST",
        "header": [
          {
            "key": "Authorization",
            "value": "Bearer {{ACCESS_TOKEN}}"
          },
          {
            "key": "Content-Type",
            "value": "application/json"
          }
        ],
        "url": {
          "raw": "https://graph.facebook.com/v19.0/{{WABA_ID}}/message_templates",
          "protocol": "https",
          "host": [
            "graph",
            "facebook",
            "com"
          ],
          "path": [
            "v19.0",
            "{{WABA_ID}}",
            "message_templates"
          ]
        },
        "body": {
          "mode": "raw",
          "raw": "{\n  \"name\": \"m1_estetica\",\n  \"language\": \"es\",\n  \"category\": \"MARKETING\",\n  \"components\": [\n    {\n      \"type\": \"BODY\",\n      \"text\": \"Hola {{1}}, en 14 días activamos 10–20 valoraciones de {{2}} sin anuncios. ¿Te va una llamada de 8 min? Agenda aquí: {{3}}\"\n    },\n    {\n      \"type\": \"FOOTER\",\n      \"text\": \"Responde STOP para dejar de recibir mensajes.\"\n    },\n    {\n      \"type\": \"BUTTONS\",\n      \"buttons\": [\n        {\n          \"type\": \"URL\",\n          \"text\": \"Abrir agenda\",\n          \"url\": \"https://calendly.com/chrisribera28/30min\"\n        }\n      ]\n    }\n  ]\n}"
        }
      }
    },
    {
      "name": "Create Template — m1_generico (MARKETING)",
      "request": {
        "method": "POST",
        "header": [
          {
            "key": "Authorization",
            "value": "Bearer {{ACCESS_TOKEN}}"
          },
          {
            "key": "Content-Type",
            "value": "application/json"
          }
        ],
        "url": {
          "raw": "https://graph.facebook.com/v19.0/{{WABA_ID}}/message_templates",
          "protocol": "https",
          "host": [
            "graph",
            "facebook",
            "com"
          ],
          "path": [
            "v19.0",
            "{{WABA_ID}}",
            "message_templates"
          ]
        },
        "body": {
          "mode": "raw",
          "raw": "{\n  \"name\": \"m1_generico\",\n  \"language\": \"es\",\n  \"category\": \"MARKETING\",\n  \"components\": [\n    {\n      \"type\": \"BODY\",\n      \"text\": \"Hola {{1}}, en 14 días activamos 10–20 citas calificadas sin anuncios. ¿Te va una llamada de 8 min? Agenda aquí: {{2}}\"\n    },\n    {\n      \"type\": \"FOOTER\",\n      \"text\": \"Responde STOP para dejar de recibir mensajes.\"\n    },\n    {\n      \"type\": \"BUTTONS\",\n      \"buttons\": [\n        {\n          \"type\": \"URL\",\n          \"text\": \"Abrir agenda\",\n          \"url\": \"https://calendly.com/chrisribera28/30min\"\n        }\n      ]\n    }\n  ]\n}"
        }
      }
    },
    {
      "name": "Create Template — m2_recordatorio (UTILITY)",
      "request": {
        "method": "POST",
        "header": [
          {
            "key": "Authorization",
            "value": "Bearer {{ACCESS_TOKEN}}"
          },
          {
            "key": "Content-Type",
            "value": "application/json"
          }
        ],
        "url": {
          "raw": "https://graph.facebook.com/v19.0/{{WABA_ID}}/message_templates",
          "protocol": "https",
          "host": [
            "graph",
            "facebook",
            "com"
          ],
          "path": [
            "v19.0",
            "{{WABA_ID}}",
            "message_templates"
          ]
        },
        "body": {
          "mode": "raw",
          "raw": "{\n  \"name\": \"m2_recordatorio\",\n  \"language\": \"es\",\n  \"category\": \"UTILITY\",\n  \"components\": [\n    {\n      \"type\": \"BODY\",\n      \"text\": \"Hola {{1}}, ¿te reservo 8 min? Mi agenda: {{2}}. Si lo prefieres, dime 2 horarios por WhatsApp.\"\n    },\n    {\n      \"type\": \"FOOTER\",\n      \"text\": \"Gracias por tu tiempo.\"\n    },\n    {\n      \"type\": \"BUTTONS\",\n      \"buttons\": [\n        {\n          \"type\": \"URL\",\n          \"text\": \"Abrir agenda\",\n          \"url\": \"https://calendly.com/chrisribera28/30min\"\n        }\n      ]\n    }\n  ]\n}"
        }
      }
    },
    {
      "name": "Create Template — noshow_reprog (UTILITY)",
      "request": {
        "method": "POST",
        "header": [
          {
            "key": "Authorization",
            "value": "Bearer {{ACCESS_TOKEN}}"
          },
          {
            "key": "Content-Type",
            "value": "application/json"
          }
        ],
        "url": {
          "raw": "https://graph.facebook.com/v19.0/{{WABA_ID}}/message_templates",
          "protocol": "https",
          "host": [
            "graph",
            "facebook",
            "com"
          ],
          "path": [
            "v19.0",
            "{{WABA_ID}}",
            "message_templates"
          ]
        },
        "body": {
          "mode": "raw",
          "raw": "{\n  \"name\": \"noshow_reprog\",\n  \"language\": \"es\",\n  \"category\": \"UTILITY\",\n  \"components\": [\n    {\n      \"type\": \"BODY\",\n      \"text\": \"¿Todo bien, {{1}}? Reprograma aquí: {{2}}. Puedo llamarte a {{3}} o {{4}}.\"\n    },\n    {\n      \"type\": \"FOOTER\",\n      \"text\": \"Te tardará menos de 1 minuto.\"\n    },\n    {\n      \"type\": \"BUTTONS\",\n      \"buttons\": [\n        {\n          \"type\": \"URL\",\n          \"text\": \"Reprogramar\",\n          \"url\": \"https://calendly.com/chrisribera28/30min\"\n        }\n      ]\n    }\n  ]\n}"
        }
      }
    },
    {
      "name": "Send — m1_generico (test)",
      "request": {
        "method": "POST",
        "header": [
          {
            "key": "Authorization",
            "value": "Bearer {{ACCESS_TOKEN}}"
          },
          {
            "key": "Content-Type",
            "value": "application/json"
          }
        ],
        "url": {
          "raw": "https://graph.facebook.com/v19.0/{{PHONE_NUMBER_ID}}/messages",
          "protocol": "https",
          "host": [
            "graph",
            "facebook",
            "com"
          ],
          "path": [
            "v19.0",
            "{{PHONE_NUMBER_ID}}",
            "messages"
          ]
        },
        "body": {
          "mode": "raw",
          "raw": "{\n  \"messaging_product\": \"whatsapp\",\n  \"to\": \"{{TEST_NUMBER}}\",\n  \"type\": \"template\",\n  \"template\": {\n    \"name\": \"m1_generico\",\n    \"language\": {\n      \"code\": \"es\"\n    },\n    \"components\": [\n      {\n        \"type\": \"body\",\n        \"parameters\": [\n          {\n            \"type\": \"text\",\n            \"text\": \"Nombre de prueba\"\n          },\n          {\n            \"type\": \"text\",\n            \"text\": \"https://calendly.com/chrisribera28/30min\"\n          }\n        ]\n      }\n    ]\n  }\n}"
        }
      }
    },
    {
      "name": "Send — m1_estetica (test)",
      "request": {
        "method": "POST",
        "header": [
          {
            "key": "Authorization",
            "value": "Bearer {{ACCESS_TOKEN}}"
          },
          {
            "key": "Content-Type",
            "value": "application/json"
          }
        ],
        "url": {
          "raw": "https://graph.facebook.com/v19.0/{{PHONE_NUMBER_ID}}/messages",
          "protocol": "https",
          "host": [
            "graph",
            "facebook",
            "com"
          ],
          "path": [
            "v19.0",
            "{{PHONE_NUMBER_ID}}",
            "messages"
          ]
        },
        "body": {
          "mode": "raw",
          "raw": "{\n  \"messaging_product\": \"whatsapp\",\n  \"to\": \"{{TEST_NUMBER}}\",\n  \"type\": \"template\",\n  \"template\": {\n    \"name\": \"m1_estetica\",\n    \"language\": {\n      \"code\": \"es\"\n    },\n    \"components\": [\n      {\n        \"type\": \"body\",\n        \"parameters\": [\n          {\n            \"type\": \"text\",\n            \"text\": \"Nombre de prueba\"\n          },\n          {\n            \"type\": \"text\",\n            \"text\": \"depilación láser\"\n          },\n          {\n            \"type\": \"text\",\n            \"text\": \"https://calendly.com/chrisribera28/30min\"\n          }\n        ]\n      }\n    ]\n  }\n}"
        }
      }
    }
  ],
  "variable": [
    {
      "key": "ACCESS_TOKEN",
      "value": "REEMPLAZA_CON_TU_TOKEN"
    },
    {
      "key": "WABA_ID",
      "value": "REEMPLAZA_CON_TU_WABA_ID"
    },
    {
      "key": "PHONE_NUMBER_ID",
      "value": "REEMPLAZA_CON_TU_PHONE_NUMBER_ID"
    },
    {
      "key": "TEST_NUMBER",
      "value": "34XXXXXXXXX"
    }
  ]
}
