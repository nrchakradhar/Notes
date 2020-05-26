# Dummies GRPC Python Example
This is simple example of grpc python.
The proto file contains a single service that calculates square root of the number.

Install grpc utilities that generate the code.
In Windows pip is present usually at C:\pathToPython\Scripts
`C:\Users\nrchakra\AppData\Local\Programs\Python\Python37-32\Scripts`

`pip3 install grpcio`

`pip3 install grpcio-tools`

The files imported in grpc server and client have to be generated using the following command.

`python -m grpc_tools.protoc -I. --python_out=. --grpc_python_out=. calculator.proto`

There are better ways to organize the folder structure instead of a single folder.

## Start server
`python grpcCalcServer.py`

```
Starting server. Listening on port 50051.
```
## Start client
`python grpcClient.py`

After the client is run, the following will appear in the server logs

```
GRPC Server SquareRoot called with: 16.0
GRPC Server SquareRoot called with: 144.0
```
