.PHONY : test1 test2 test3

define func1
	@echo "My name is $(0)"
endef

define func2
	@echo "My name is $(0)"
	@echo "    Param 1 => $(0)"
	@echo "    Param 2 => $(1)"
endef


var := $(call func1)
new := $(func1)


test1 :
	$(call func1)
	$(call func2)

test2 :
	$(call func2,param)

test3 :
	@echo "var => $(var)"
	@echo "new => $(new)"