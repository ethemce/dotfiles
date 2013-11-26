Installation:
	
	git clone https://github.com/kodbank/dotfiles ~/dotfiles

Symlinks:

	ln -s ~/dotfiles/vim/ ~/.vim
	ln -s ~/dotfiles/vim/vimrc ~/.vimrc
	
	ln -s ~/dotfiles/bash/bashrc ~/.bashrc
	ln -s ~/dotfiles/bash/profile ~/.bash_profile  #mac
	ln -s ~/dotfiles/bash/aliases ~/.bash_aliases


VCPrompt:

	mkdir -p ~/bin
	curl -sL https://raw.github.com/djl/vcprompt/master/bin/vcprompt > ~/bin/vcprompt
	chmod 755 ~/bin/vcprompt
	

exuberant-ctags:

	sudo aptitude install exuberant-ctags
	

Git submodule update

	cd ~/dotfiles/
	git submodule update --init

Django tab-completion feature:

	ln -s ~/dotfiles/utils/django_completion.sh ~/.django_completion

Source:

	source ~/.bashrc
	source ~/.bash_profile  #mac
