OPTS= -g -Wall -ansi -pedantic -std=c++20

OBJS = main.o AVLTree.o AVLNode.o

CC = g++ -c $(OPTS) 
LN = g++

AVLtest: $(OBJS)
	$(LN) -o AVLtest $(OBJS)

main.o: main.cpp AVLTree.hpp AVLNode.hpp
	$(CC) main.cpp

AVLTree.o: AVLTree.cpp AVLTree.hpp AVLNode.hpp
	$(CC) AVLTree.cpp

AVLNode.o: AVLNode.cpp AVLNode.hpp
	$(CC) AVLNode.cpp

clean:
	/bin/rm -f $(OBJS) AVLtest *~

