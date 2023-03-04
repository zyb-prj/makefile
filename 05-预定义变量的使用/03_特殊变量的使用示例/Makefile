
.PHONY : add out first second third test

all out :
	@echo "$(MAKE)"
	@echo "$(MAKECMDGOALS)"
	@echo "$(MAKEFILE_LIST)"
	@echo "$(MAKE_VERSION)"
	@echo "$(CURDIR)"
	@echo "$(.VARIABLES)"

first :
	@echo "first"
second :
	@echo "second"
third :
	@echo "third"

test :
	@$(MAKE) first
	@$(MAKE) second
	@$(MAKE) third

