https://docs.docker.com/registry/insecure/
openssl req \
  -newkey rsa:4096 -nodes -sha256 -keyout certs/domain.key \
  -addext "subjectAltName = DNS:registry" \
  -x509 -days 365 -out certs/domain.crt

//sudo chown -R vscode:rustlang /usr/local/cargo