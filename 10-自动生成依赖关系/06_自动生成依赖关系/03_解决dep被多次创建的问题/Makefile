.PHONY : all clean

MKDIR := mkdir
RM := rm -fr
CC := gcc

DIR_DEPS := deps

SRCS := $(wildcard *.c)
DEPS := $(SRCS:.c=.dep)
DEPS := $(addprefix $(DIR_DEPS)/, $(DEPS))

ifeq ("$(MAKECMDGOALS)", "all")
include $(DEPS)
endif

all :
	@echo "all"

$(DIR_DEPS) :
	$(MKDIR) $@

ifeq ("$(wildcard $(DIR_DEPS))", "")
$(DIR_DEPS)/%.dep : $(DIR_DEPS) %.c
else
$(DIR_DEPS)/%.dep : %.c
endif
	@echo "Creating $@ ..."
	@set -e; \
	$(CC) -MM -E $(filter %.c, $^) | sed 's,\(.*\)\.o[ :]*,objs/\1.o : ,g' > $@

clean :
	$(RM) $(DIR_DEPS)