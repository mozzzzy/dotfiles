.PHONY: install
install: preinstall install_zshrc install_zsh-autosuggestions install_zsh-git-prompt

.PHONY: preinstall
preinstall:
	mkdir -p ~/zsh

.PHONY: install_zshrc
install_zshrc: zshrc
	cp $^ ~/.$^

.PHONY: install_zsh-autosuggestions
install_zsh-autosuggestions: zsh-autosuggestions/zsh-autosuggestions.zsh
	cp $^ ~/zsh/.zsh-autosuggestions.zsh

.PHONY: install_zsh-git-prompt
install_zsh-git-prompt: zsh-git-prompt
	cp -r $^ ~/zsh/

.PHONY: clean
clean:
	rm -rf \
		~/.zshrc \
		~/zsh
