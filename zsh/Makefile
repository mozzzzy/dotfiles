.PHONY: install
install: preinstall install_zshrc install_zshrc_parts install_zlogout install_zsh-autosuggestions install_git_prompt_sh install_zsh_syntax-highlighting

.PHONY: preinstall
preinstall:
	mkdir -p ~/zsh

.PHONY: install_zshrc
install_zshrc: zshrc
	cp $^ ~/.$^

.PHONY: install_zshrc_parts
install_zshrc_parts: zshrc_parts
	cp -r $^ ~/zsh/$^

.PHONY: install_zlogout
install_zlogout: zlogout
	cp $^ ~/.$^

.PHONY: install_zsh-autosuggestions
install_zsh-autosuggestions: zsh-autosuggestions/zsh-autosuggestions.zsh
	cp $^ ~/zsh/.zsh-autosuggestions.zsh

.PHONY: install_git_prompt_sh
install_git_prompt_sh: git-prompt.sh
	cp $^ ~/.$^

.PHONY: install_zsh_syntax-highlighting
install_zsh_syntax-highlighting: zsh-syntax-highlighting
	cp -r $^ ~/zsh/

.PHONY: clean
clean:
	rm -rf \
		~/.zshrc \
		~/zsh
