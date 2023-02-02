# Examples for accessing the mission‹one› REST API
This page contains examples of using the mission‹one› REST API via common programming languages.
The examples are written in C#, Java and Python.

## The Authorization Header
When creating a new apikey, an Authorization header will be provided to you via the mission‹one› dialog+ or our customer support. This header will look something like this...
```
Authorization: Bearer eyJhbG[...]XVCJ9.eyJ2IjoiMS4wI[...]iaXNzIjoiTTFSZXN0QVBJcyJ9.FRLWBEO[...]tg72ZIwM
```
...and has to be passed as an Authorization HTTP-header like in the following example.

```
curl --location --request GET 'https://CloudApi.mission-one.de/Rest/Subscribers/subscriberimports/{importId}/result' 
--header 'Authorization: Bearer eyJhbG[...]XVCJ9.eyJ2IjoiMS4wI[...]iaXNzIjoiTTFSZXN0QVBJcyJ9.FRLWBEO[...]tg72ZIwM'
```

