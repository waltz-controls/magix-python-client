# magix-python-client

Python client implementation for Magix

## Usage

```
pip install magix_client
```

```
magix_host = 'http://magix:8080'

#create instance
client = MagixHttpClient(magix_host)
#
client.observe().subscribe(lambda event: print(json.loads(event.data)))
client.broadcast({'hello':'world'})
```
