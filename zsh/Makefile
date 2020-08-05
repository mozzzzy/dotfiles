.PHONY: install
install: preinstall install_zshrc install_zlogout install_zsh-autosuggestions install_git_prompt_sh

.PHONY: preinstall
preinstall:
	mkdir -p ~/zsh

.PHONY: install_zshrc
install_zshrc: zshrc
	cp $^ ~/.$^

.PHONY: install_zlogout
install_zlogout: zlogout
	cp $^ ~/.$^

.PHONY: install_zsh-autosuggestions
install_zsh-autosuggestions: zsh-autosuggestions/zsh-autosuggestions.zsh
	cp $^ ~/zsh/.zsh-autosuggestions.zsh

.PHONY: install_git_prompt_sh
install_git_prompt_sh: git-prompt.sh
	cp $^ ~/.$^

.PHONY: clean
clean:
	rm -rf \
		~/.zshrc \
		~/zsh
