https://www.redhat.com/sysadmin/replace-docker-podman-macos

### Add to .zshrc
export CONTAINER_HOST=ssh://vagrant@127.0.0.1:2222/run/podman/podman.sock
export CONTAINER_SSHKEY=/Users/[username]/tools/podman/.vagrant/machines/default/virtualbox/private_key

### Gotchas
Using homebrew to install Podman may result in a Podman version that is incompatible with the latest Podman release used in Fedora 32.
Solution: Swap the box in your Vagrantfile to fedora/34-cloud-base or newer.

