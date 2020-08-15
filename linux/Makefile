generate_ssh_key:
	ssh-keygen -t rsa  

get_ssh_key:
	cat /home/osboxes/.ssh/id_rsa.pub

vim:
	sudo apt-get install vim -y

install_vim_plug:
	curl -fLo ~/.vim/autoload/plug.vim --create-dirs https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim

asdf_install:
	git clone https://github.com/asdf-vm/asdf.git ~/.asdf --branch v0.8.0-rc1
	echo '. $$HOME/.asdf/asdf.sh' >> bashrc
	source ~/.bashrc
