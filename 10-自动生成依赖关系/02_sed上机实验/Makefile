.PHONY : echo_only_single echo_only_sed echo_relay_single echo_relay_sed echo_relay_path_sed

echo_only_single :
	echo "test=>abc+abc=abc"

echo_only_sed :
	echo "test=>abc+abc=abc" | sed 's:abc:xyz:g'

echo_relay_single :
	echo "main.o : main.c func.h"

echo_relay_sed :
	echo "main.o : main.c func.h" | sed 's,\(.*\)\.o[ :]*,objs/\1.o : ,g'

echo_relay_objs_sed :
	echo "/a/b/c/d/main.o : main.c func.h" | sed 's,\(.*\)\.o[ :]*,objs/\1.o : ,g'

echo_relay_xyz_sed :
	echo "a/b/c/d/main.o : main.c func.h" | sed 's,\(.*\)\.o[ :]*,xyz/\1.o : ,g'

echo_relay_symbol_sed :
	echo "a/b/c/d/main.o :::::::: main.c func.h" | sed 's,\(.*\)\.o[ :]*,xyz/\1.o : ,g'