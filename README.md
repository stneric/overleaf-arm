# overleaf-arm

Running Overleaf (ShareLaTeX) on ARM devices

# Usage

As described [here](https://shihabkhan1.github.io/overleaf/intro.html), the standard setup works for x86/x64 systems but unfortunately not for ARM systems out of the box. The setup process described below is straightforward.

You will need:

*   Docker
*   The Overleaf repository (`git clone https://github.com/overleaf/overleaf.git`)
*   The `docker-compose.yml` file from this repository

Replace the default `docker-compose.yml` in the `overleaf` directory with the one provided here, then run:
`docker compose up -d`

## Additional Information

After the containers are running, access the `sharelatex` container's shell and run `tlmgr install scheme-full` to install the complete TeX Live distribution.

### Notes 

- The overleaf container will run emulated as currently only an amd64 image is provided by overleaf.
- All the premium features are commented out. If they aren't, documents in overleafs GUI won't compile
