## Conversation Assistant

The purpose of the Conversation Assistant is to help and guide users in finding answers to the most frequent asked questions about the OpertusMundi marketplace. 
An conversation assistant can improve the user experience by interacting with 
the users, understanding their questions and providing answers to them.



### Requirements:
* Python 3.8.5

To install the required libraries, simply run: 

```
pip install -r requirements.txt
python -m spacy download en_core_web_md
```

### Intereact with the Conversation Assistant locally
Intereact with the conversation assistant by executing the following from project root directory:
```
rasa x
```
Then the Rasa X UI will run locally at http://localhost:5002/login?username=me&password=KoVg01ePU3Zb.

### Connect external channels

For details of the deployment of Rasa X on a server as a set of Docker containers, please see https://rasa.com/docs/rasa-x/installation-and-setup/install/docker-compose/



<br/><br/>


### Dialogue example<br/><br/>
<img src="https://github.com/OpertusMundi/intelligent-search-assistant/blob/main/image/rasa_x.png"></img><br>



