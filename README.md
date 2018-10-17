# SPACY NLP issues

## Prerequisities

see https://github.com/kengz/spacy-nlp/blob/master/README.md

## Installation

* `npm install`

## Running

* `npm run spacy` - spacy server
* `npm start` - client (test string nlp)

## Expected results

Per https://github.com/kengz/spacy-nlp/blob/master/README.md

## Actual results

* it is not working - getting null as result at https://github.com/alivanov/spacy-nlp-issue/blob/master/index.js#L6
* workaround - https://github.com/kengz/spacy-nlp/issues)

## Troubleshooting

* ensure you're using python3 (https://stackoverflow.com/questions/18425379/how-to-set-pythons-default-version-to-3-x-on-os-x)
* python3 -m pip install -U socketIO-client-nexus
* update node_modules/spacy-nlp/src/client.py#13 to be `from socketIO_client_nexus import SocketIO, WebsocketTransport`
* restart the spacy server
