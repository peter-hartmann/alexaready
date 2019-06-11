# Simple Alexa App

JSON
```
{
    "interactionModel": {
        "languageModel": {
            "invocationName": "ready",
            "intents": [
                {
                    "name": "nameIntent",
                    "slots": [
                        {
                            "name": "NAME",
                            "type": "AMAZON.US_FIRST_NAME"
                        }
                    ],
                    "samples": [
                        "my name is {NAME}",
                        "my name's {NAME}",
                        "set my name to {NAME}"
                    ]
                },
                {
                    "name": "AMAZON.NavigateHomeIntent",
                    "samples": []
                }
            ],
            "types": []
        }
    }
}
```