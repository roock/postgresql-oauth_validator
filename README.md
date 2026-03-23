# Postgresql oauth2 validator Debian Repository

## How to use
Run the following command:
```bash
sudo wget https://roock.github.io/postgresql-oauth_validator/repo.asc -O /usr/share/keyrings/postgresql-oauth2-validator-keyring.asc \
  && echo "deb [signed-by=/usr/share/keyrings/postgresql-oauth2-validator-keyring.asc] https://roock.github.io/postgresql-oauth_validator $(. /etc/os-release; echo "${UBUNTU_CODENAME:-${DEBIAN_CODENAME:-${VERSION_CODENAME}}}") main" | sudo tee /etc/apt/sources.list.d/postgresql-oauth-validator.list \
  && sudo apt update \
  && sudo apt install postgresql-18-oauth-validator
```
