# online-tools

* Vagrant setup
```sh
vagrant init
vagrant box add hashicorp/bionic64 --force
```

* When run `vagrant up` got this error:
```code
An error occurred while downloading the remote file. The error
message, if any, is reproduced below. Please fix this error and try
again.
Couldn't open file /Users/heguowei/www/hegwout.github.io/base
```

vi Vagrantfile
replace  config.vm.box = "base"
with  config.vm.box = "hashicorp/bionic64"

resolved this issue.

* Vagrant start up
```sh
vagrant up
vagrant ssh
```

* Vagrant reload & provision to install packages
```
vagrant reload
vagrant provision
```