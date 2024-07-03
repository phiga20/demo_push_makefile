.PHONY: ALL
#gan cac bien cc = gcc and include các file.h
CC := gcc
INC_FILE := ./include/hieu.h
INC_FILE += ./include/tong.h
#-c chi dinh qua trinh biên dịch và tạo đối tượng nhưng không linking.
%.o: $(INC_FILE)
	$(CC) -c src/hieu.c -o obj/hieu.o -I./include
	$(CC) -c src/tong.c -o obj/tong.o -I./include
	$(CC) -c main.c -o obj/main.o -I./include
#linking cac file.o tao ra file exe
tong: obj/tong.o obj/main.o
	$(CC) obj/tong.o obj/main.o -o bin/out.exe

hieu: obj/hieu.o obj/main.o
	$(CC) obj/hieu.o obj/main.o -o bin/out.exe
#chay fiel.exe
run:
	.\bin\out.exe

clean:
	rm ./obj/*.o