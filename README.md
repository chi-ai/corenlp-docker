# corenlp-docker
corenlp-docker provides a dockerised version of the [Stanford CoreNLP Server](https://stanfordnlp.github.io/CoreNLP/corenlp-server.html).

## Building the image

```
docker build -t mycorenlp .
docker run -d --restart unless-stopped -p 9000:9000 mycorenlp
```

## Simple usage

To pull the image and start the server, run:
```
curl --data 'A rather short sentence.' http://localhost:9000
```

For more complex examples of using the API, please refer to
[the official documentation](https://stanfordnlp.github.io/CoreNLP/corenlp-server.html) of CoreNLP Server.
