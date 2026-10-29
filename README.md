# Dealer Evaluation Frontend

Course starter: https://github.com/ibm-developer-skills-network/dealer_evaluation_frontend

The course frontend loads products, lists their dealers, and shows an individual
dealer's price or a table of all available prices. Product changes clear the
previous dealer selection and price.

## Current status

The local preview uses the Product Details API on port 5100 and Dealer Pricing
API on port 5180. Browser checks verified Laptop pricing for Tech City ($850)
and all dealers ($850, $1000 and $1500).

Code Engine deployment is pending course-provided access. The URLs in
`html/index.html` are local preview endpoints, not deployed Code Engine URLs.
Replace `produrl` and `dealerurl` with the real backend URLs after deployment.

## Local run

Install `requirements.txt` into a Python environment. Start both backend APIs,
then run this command from this repository:

```text
python -m flask --app app run --host=127.0.0.1 --port=5101 --no-reload
```

Open http://127.0.0.1:5101/ to test the integration. The frontend container uses port 5001.
