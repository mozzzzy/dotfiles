.PHONY: install
install: install_vimrc install_autoload install_colors install_templates

.PHONY: install_vimrc
install_vimrc: vimrc
	mkdir -p ~/.vim
	cp vimrc ~/.vim/

.PHONY: install_autoload
install_autoload: $(wildcard autoload/*)
	mkdir -p ~/.vim/autoload
	cp $^ ~/.vim/autoload/

.PHONY: install_colors
install_colors: $(wildcard colors/*)
	mkdir -p ~/.vim/colors
	cp $^ ~/.vim/colors/

.PHONY: install_templates
install_templates: $(wildcard templates/*)
	mkdir -p ~/.vim/templates
	cp $^ ~/.vim/templates/
