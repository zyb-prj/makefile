OBJS := func.o main.o

$(OBJS) : %.o : %.c
	gcc -o $@ -c $^

	||
	||
	--

func.o : func.c
	gcc -o $@ -c $^

main.o : main.c
	gcc -o $@ -c $^