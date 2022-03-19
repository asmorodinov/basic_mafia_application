# basic_mafia_application

Пример запуска сервера в докере (работает немного странно)

```
docker run -p 8888:5000 -p 1111:50051 -i asmorodinov/basic_mafia_application  
```
```
Enter port number to run on --> 5000
Initialized voice chat server
Running on IP: 172.17.0.2
Running on port: 5000
INFO:root:Starting server
Select port to run server on (e.g. 50051): 50051
```

Если запускать просто на локальной машине, то два сервера (voice chat и мафия) получают разные ip адреса и всё прекрасно работает.

Например:
```
python3 mafia_server.py
Enter port number to run on --> 5000
Initialized voice chat server
Running on IP: 172.21.240.1
Running on port: 5000
INFO:root:Starting server
Select port to run server on (e.g. 50051): 50051
```