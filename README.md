# Nota
See [Lanhild/ppa-maintainers](https://github.com/Lanhild/ppa-maintainers/README.md) for further details.

# Usage
The `gen-release` creates a release following [Debian packaging conventions](https://wiki.debian.org/Packaging).
`prod-release` is used to push source code changes upstream.

# Add the repository to your local sources
```bash
sudo apt install apt-transport-https curl

sudo curl -fsSLo /etc/apt/trusted.gpg.d/numigi-ppa-keyring.asc https://lanhild.github.io/numigi-ppa/KEY.asc

echo 'deb [signed-by=/etc/apt/trusted.gpg.d/numigi-ppa-keyring.asc arch=amd64] https://lanhild.github.io/numigi-ppa/ ./' |sudo tee /etc/apt/sources.list.d/numigi_ppa.list

sudo apt update
```