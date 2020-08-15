asdf_list_versions:
	asdf list all ruby

asdf_install_ruby_1_9_3:
	asdf plugin add ruby
	sudo apt purge libssl-dev && sudo apt install libssl1.0-dev -y
	asdf install ruby 1.9.3-p551

asdf_install_ruby_2_4_0:
	sudo apt purge libssl-dev && sudo apt install libssl1.0-dev -y
	asdf install ruby 2.4.0

asdf_use:
	asdf global ruby $(version)
