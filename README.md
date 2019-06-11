# Simple Alexa App

1. Install [nodejs](https://nodejs.org/en/download/) and [yarn](https://yarnpkg.com/en/docs/install#windows-stable)

1. Clone the project, build and run

        git clone https://github.com/peter-hartmann/alexaready.git
        cd alexaready
        yarn
        yarn start

1. Configure reverse proxy

1. In [Alexa Development Console](https://developer.amazon.com/alexa/console/ask) use configure the endpoint HTTPS

1. In [Alexa Development Console](https://developer.amazon.com/alexa/console/ask) use JSON Editor and replace JSON with:

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
