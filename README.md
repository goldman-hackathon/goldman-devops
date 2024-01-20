# Odpalanie aplikacji

1. Budujemy obrazy Dockerowe
```
docker build -t goldman-back -f <sciezka do goldman-back>/Dockerfile <sciezka do goldman-back>

docker build -t goldman-front -f <sciezka do goldman-front>/Dockerfile <sciezka do goldman-front>
```
na przykład u mnie
```
docker build -t goldman-back -f ../goldman-back/Dockerfile ../goldman-back

docker build -t goldman-front -f ../goldman-front/Dockerfile ../goldman-front
```

2. uruchamiamy aplikację
```
docker-compose -f <ścieżka do docker-compose> up
```
na przykład u mnie
```
docker-compose -f ./docker-compose.yml up
```

3. Korzystamy z aplikacji :D

w przeglądarce odpali się pod adresem `localhost:3000`