
.PHONY : GCC-M-SINGLE GCC-MM-SINGLE GCC-M-E-PREFIX GCC-M-E-PREFIX

GCC-M-SINGLE :
	gcc -M main.c

GCC-MM-SINGLE :
	gcc -MM main.c

GCC-M-E-PREFIX :
	gcc -M -E main.c | sed 's,\(.*\)\.o[ :]*,objs/\1.o : ,g'

GCC-MM-E-PREFIX :
	gcc -MM -E main.c | sed 's,\(.*\)\.o[ :]*,objs/\1.o : ,g'