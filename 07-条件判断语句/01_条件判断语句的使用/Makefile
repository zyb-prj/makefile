.PHONY : test

var1 := A
var2 := $(var1)
var3 :=

test:
    ifeq ($(var1),$(var2))
		@echo "var1 == var2"
    else
		@echo "var1 != var2"
    endif

    ifneq ($(var2),)
		@echo "var2 is NOT empty"
    else
		echo "var2 is empty"
    endif

    ifdef var2
		@echo "var2 is NOT empty"
    else
		echo "var2 is empty"
    endif

    ifndef var3
		echo "var3 is empty"
    else
		@echo "var2 is NOT empty"
    endif