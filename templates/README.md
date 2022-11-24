https://docs.docker.com/registry/insecure/
openssl req \
  -newkey rsa:4096 -nodes -sha256 -keyout certs/domain.key \
  -addext "subjectAltName = DNS:registry" \
  -x509 -days 365 -out certs/domain.crt

//sudo chown -R vscode:rustlang /usr/local/cargo

docker logs -n 100 35ee0cbd06e1 2>&1 | grep "PUB"

docker logs -n 1000 35ee0cbd06e1 2>&1 | grep "SUB"

docker logs -n 6000 b2c6a34c034d 2>&1 | grep "welcome"

docker logs -n 1000 35ee0cbd06e1 2>&1 | grep "AAA"

docker logs -n 6000 983e09e41e0d 2>&1 | grep "help"

docker logs -n 200 2de6af269e67

docker stop $(docker ps -a -q)
docker rm $(docker ps -a -q)