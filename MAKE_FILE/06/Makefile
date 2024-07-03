#makefile mo ta qua trinh bien dịch và linker cua mot chuong trinh c.
.PHONY: stage1 stage2 stage3 stage4 all clean
# -E chi định giai đoạn tiền xử lý tạo ra các file.i. 
stage1:
	gcc -E hello.c -o hello.i
# -s chi định giai đoạn compiler để tạo ra ngôn ngữ asemberly.
stage2:
	gcc -S hello.i -o hello.s
#-c chi dinh qua trinh biên dịch và tạo đối tượng nhưng không linking.
stage3:
	gcc -c hello.s -o hello.o
#-o linking ca fil.o tao ra file thuc thi.
stage4:
	gcc hello.o -o hello
all:
	gcc hello.c -o hello
clean:
	rm -rf hello hello.i hello.s hello.o