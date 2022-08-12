
# Build

```
yarn
yarn build
```

# Testing

First, you need to install `ipyeos`.

```
python3 -m pip install -U ipyeos
```

Then run the test server:
```
eos-debugger
```

Also, you can run `eos-debugger` in a docker container.

First, pull the docker image:

```
docker pull ghcr.io/uuosio/ipyeos:latest
```

Run eos-debugger in a docker container:
```
docker run -it --rm -p 9090:9090 -p 9092:9092 -p 9093:9093 -t ghcr.io/uuosio/ipyeos
```

Finally, run the test:
```
yarn test
```