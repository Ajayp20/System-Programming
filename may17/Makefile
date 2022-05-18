CC = g++
BIN = bin/
OBJ = obj/
INC = include/
SRC = src/
CFLAG = -c
OFLAG = -o
all: clean build-server build-client

build-server: $(OBJ)func.o
	$(CC) $(OFLAG) $(BIN)server20 $(SRC)server.cpp $(OBJ)func.o
$(OBJ)func.o:
	$(CC) $(CFLAG) $(OFLAG) $(OBJ)func.o $(SRC)func.cpp
      
build-client:
	$(CC) $(OFLAG) $(BIN)client20 $(SRC)client.cpp
    
start-server:
	./$(BIN)server20
 
start-client:
	./$(BIN)client20
       
clean:
	rm $(OBJ)func.o
	rm $(BIN)client20
	rm $(BIN)server20
  
