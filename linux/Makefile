generate_ssh_key:
	ssh-keygen -t rsa  

get_ssh_key:
	cat ~/.ssh/id_rsa.pub

vim_install:
	sudo apt-get install vim -y
	git clone git@github.com:rogesson/dotfiles.git ~/dotfiles
	cp templates/vim/.vimrc ~/.vimrc

vim_plug_install:
	curl -fLo ~/.vim/autoload/plug.vim --create-dirs https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim

asdf_install:
	git clone https://github.com/asdf-vm/asdf.git ~/.asdf --branch v0.8.0-rc1
	echo '. $(HOME)/.asdf/asdf.sh' >> bashrc
	. $(HOME)/.asdf/asdf.sh
	source ~/.bashrc

