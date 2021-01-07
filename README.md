# Intelligent Search Assistant

The purpose of the Intelligent Search Assistant is to help and guide users in finding the most relevant 
assets in the OpertusMundi marketplace. 
An intelligent search assistant can significantly improve the search experience by interacting with 
the user and understanding their query to provide better results, and integrating in the provided resources the 
rich information in terms of metadata and automated metadata produced and managed by the marketplace. 

# Setup

##### Prerequisites
* Python 3.6
* Rasa and Rasa X

```
pip install rasa-x --extra-index-url https://pypi.rasa.com/simple
```

##### Run Conversation Assistant
Run the Conversation Assistant by executing the following from project root directory:
```
rasa run --enable-api
```

## Documentation

Once the server is running at http://localhost:5005, access the chatbot via REST endpoint:

#### POST /webhooks/rest/webhook
##### Sample Body
```json
{
  "sender": "some_id",
  "message": "Hello!"
}
```
##### Sample Response
```json
[
    {
        "recipient_id": "some_id",
        "text": "Hey! How are you?"
    }
]
```

## Training NLU

To train the NLU models via Rasa X UI, run the following from project root directory:
```
rasa x
```

Then the Rasa X training UI will run at http://localhost:5002