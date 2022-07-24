# LINE TOWN election

## Run via docker
Let’s run the server automatically via docker-compose:

```sh
docker-compose -p local -f ./docker-compose.yml up -d
```

Let’s go to: http://localhost:3000/

see the [README.md](README.md) file in client or server for more details

## Usage

### Stage 1 - open the Election

```sh
curl -X POST {endpoint}/api/election/toggle -H 'Content-Type: application/json' -d '{"enable":true}'

# example
curl -X POST http://localhost:8000/api/election/toggle -H 'Content-Type: application/json' -d '{"enable":true}'
```

### Stage 2 - vote in web

you can delete the local storage data if you want to vote new national id

### Stage 3 - close the Election

```sh
curl -X POST {endpoint}/api/election/toggle -H 'Content-Type: application/json' -d '{"enable":false}'

# example
curl -X POST http://localhost:8000/api/election/toggle -H 'Content-Type: application/json' -d '{"enable":false}'
```

<!-- CONTACT -->
## Contact

* **Tanawat Hongthai** - *tana.h@kkumail.com* - [Lazts](https://lazts.com)

<!-- LICENSE -->
## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
