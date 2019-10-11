### Hackering

1. npm install
2. docker-compose up -d
3. docker inspect -f '{{range .NetworkSettings.Networks}}{{.IPAddress}}{{end}}' $(docker-compose ps | awk '/untitledelements/{print$1}')
