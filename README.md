# Playbooks

## Getting started

* Install python
* Install ansible (through pip3 to avoid issues with apt update)
* ```sh ansible-galaxy install -r required-roles.yml```
* ```sh ansible ```

```sh ansible-playbook -i inventory playbooks/dev-env.yaml -K```

## All playbooks

### Environment setup

playbooks/dev-env.yaml

Software:
    - go
    - kind
    - kubectl
    - hugo
    - emacs
    - docker
    - kustomize
    - git
Configuration:
    - dotfiles
    - emacs

## Testing Playbooks with Vagrant & Virtualbox

* Download [vagrant](https://www.vagrantup.com/downloads.html) and put it somewhere on your path.
* Install virtual box: ```sh sudo apt install virtualbox```
* Configure the desired playbook in the Vagrantfile
* ```sh vagrant up```
* ```sh vagrant provision```

To terminate the VM after testing run: ```sh vagrant destroy```.


