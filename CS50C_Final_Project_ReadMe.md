# DNS Redirection Demo (CS50 Cybersecurity)

## Ethical Disclaimer
This project is an educational simulation performed in a local, isolated environment.
It does not target real domains, real organizations, or real users. The demo domain
`realbank.test` is fictional and used only for local testing.

## What this demonstrates
- How "DNS redirection" can cause a user to reach a lookalike website
- Why HTTPS/TLS and X.509 certificates matter (certificate validation warnings)
- Integrity risks when name resolution is compromised

## Requirements
- Python 3.10+
- `pip install -r requirements.txt`

## How to run (HTTP demo)
Terminal 1:
python legit_server.py

Terminal 2:
python evil_server.py

Terminal 3:
python client.py

## Optional: HTTPS certificate demo
1) Generate a self-signed certificate:
python generate_cert.py

2) Run the HTTPS clone server:
python evil_https_server.py

Open:
https://127.0.0.1:8443
You should see a browser warning because the certificate is self-signed.

## Notes
This project models the threat class (DNS redirection) without modifying any real DNS
infrastructure. The "DNS" behavior is simulated inside `client.py`.# CS50
All CS50 works are stored here
