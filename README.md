# GoAlert

## Start

```bash
docker-compose up
```

## Create Users

```bash
docker exec -it goalert-goalert-1 goalert add-user --admin --user admin --pass 12345678
```

## Setup GoAlert

Use the [setup wizard](http://localhost:8081/wizard)

## Create alerts

```bash
curl -XPOST "http://localhost:8081/api/v2/generic/incoming?token=9f57cb9e-f954-404a-98bc-6686fb9c7a7c&summary=test&details=test"
```

NOTE: _token need to be changed obviously_
