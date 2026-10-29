# Dealer Evaluation Frontend

Course starter: https://github.com/ibm-developer-skills-network/dealer_evaluation_frontend

The course frontend loads products, lists their dealers, and shows an individual
dealer's price or a table of all available prices. Product changes clear the
previous dealer selection and price.

## Current status

The frontend and both backend services are deployed on IBM Code Engine.
`html/index.html` uses the real HTTPS backend URLs.

Application: https://dealer-evaluation.2giim37ib6oe.us-south.codeengine.appdomain.cloud/

Live API checks passed for four products, twelve individual dealer prices,
four complete price lists, and cross-origin access. Browser checks verified
Laptop pricing for Tech City ($850) and all dealers ($850, $1000 and $1500).

## Local run

Install `requirements.txt` into a Python environment. Start both backend APIs,
then run this command from this repository:

```text
python -m flask --app app run --host=127.0.0.1 --port=5101 --no-reload
```

Open http://127.0.0.1:5101/ to test the integration with the deployed APIs.
The frontend container uses port 5001.
