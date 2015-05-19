Installation:

Aptitude:

	sudo aptitude install exuberant-ctags curl git sudo

VCPrompt:

	mkdir -p ~/bin
	curl -sL https://raw.github.com/djl/vcprompt/master/bin/vcprompt > ~/bin/vcprompt
	chmod 755 ~/bin/vcprompt

Git submodule update
	git clone https://github.com/kodbank/dotfiles ~/dotfiles;
	cd ~/dotfiles/
	git submodule update --init


Symlinks:
	
	ln -s ~/dotfiles/vim/ ~/.vim
	ln -s ~/dotfiles/vim/vimrc ~/.vimrc
	
	rm ~/.bashrc; ln -s ~/dotfiles/bash/bashrc ~/.bashrc
	ln -s ~/dotfiles/bash/aliases ~/.bash_aliases
	ln -s ~/dotfiles/bash/profile ~/.bash_profile  #mac
	

Django tab-completion feature:

	ln -s ~/dotfiles/utils/django_completion.sh ~/.django_completion

Source:

	source ~/.bashrc
	source ~/.bash_profile  #mac
