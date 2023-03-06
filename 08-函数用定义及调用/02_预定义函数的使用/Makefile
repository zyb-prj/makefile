.PHONY : test

define func1
	@echo "My name is $(0)"
endef

define func2
	@echo "My name is $(0)"
endef

var1 :=$(call func1)
var1 :=$(call func2)
var3 := $(abspath ./)
var4 :=$(abspath hello.c)

test :
	@echo "var1 => $(var1)"
	@echo "var2 => $(var2)"
	@echo "var3 => $(var3)"
	@echo "var4 => $(var4)"