.PHONY: install
install: install_bash_profile install_git_prompt_sh

.PHONY: install_bash_profile
install_bash_profile: bash_profile
	cp $^ ~/.$^

.PHONY: install_git_prompt_sh
install_git_prompt_sh: git-prompt.sh
	cp $^ ~/.$^
