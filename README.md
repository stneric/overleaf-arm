# overleaf-arm
Fixing overleaf (sharelatex) for ARM devices

# Usage
As written up here: https://shihabkhan1.github.io/overleaf/intro.html it works for x86/x64 systems but sadly not for ARM, at least not out of the box.
The installation is pretty straight forward.

You'll need:
- Docker
- The overleaf repository (`git clone https://github.com/overleaf/overleaf.git`)
- my docker compose yaml

Just replace the docker compose with the one in this repository and 
`docker compose up -d`
