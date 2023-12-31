# Terminologies in NoSQL

## Scalability

It refers to how easily a database can expand its hardware usage

### Vertical Scalability

It refers to the ease of adding more processing power i.e. CPU and RAM

### Horizontal Scalability

It refers to the ease of adding more systems/servers

## Javascript Object Notation (JSON)

- A JSON is an object with key value pairs and can have objects within object

- It is used in Document based NoSQL databases

```JSON
{
    "ID": "1",
    "nickname": "ChosenOne9000",
    "name":"Anakin Skywalker",
    "address":
    {
        "locality": "Jedi Temple",
        "district": "Temple Precinct",
        "planet": "Coruscant"
    }
}
```

- Here, another object may have country in address as well and no rules will be
broken

## Auto Replication

Whenever a failure occurs, data replicates itself to a previous consistent state.
