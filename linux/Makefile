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
	echo '. $(HOME)/.asdf/asdf.sh' >> bashrc'
	echo '-e "\n. $(HOME)/.asdf/asdf.sh" >> ~/.zshrc
	. $(HOME)/.asdf/asdf.sh
	source ~/.bashrc

asdf_update:
	asdf plugin-update ruby

docker_install:
	sudo apt update
	sudo apt install apt-transport-https ca-certificates curl software-properties-common
	curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
	sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu bionic stable"
	sudo apt update
	apt-cache policy docker-ce
	sudo apt install docker-ce
	sudo systemctl status docker
	sudo groupadd docker
	sudo gpasswd -a $USER docker
	sudo usermod -aG docker $USER
	newgrp docker
	sudo service docker restart

docker_compose_install:
	sudo curl -L https://github.com/docker/compose/releases/download/1.26.0/docker-compose-`uname -s`-`uname -m` -o /usr/local/bin/docker-compose
	sudo chmod +x /usr/local/bin/docker-compose
	docker-compose --version

oh_my_zsh:
	sudo apt-get install zsh
	sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

install_terminator:
	sudo apt-get install terminator

install_chromium:
	sudo apt install chromium-browser
