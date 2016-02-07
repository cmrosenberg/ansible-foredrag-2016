# Hva viste jeg her?

* `vagrant up` for å starte den virtuelle maskinen.
* `ansible-playbook setup/setup.yml --limit vagrant` for å kjøre oppsett-scriptet på Vagrant-maskinen.
* `ansible-playbook setup/setup.yml --limit digitalocean` for å kjøre oppsett-scriptet på Digital Ocean-serveren.

## Noe gikk galt under foredraget. Hva skjedde?

Vagrantfilen kjørte nyeste Ubuntu, mens Digital Ocean-serveren kjørte Ubuntu 14.04. Disse opererer med forskjellige paths for hvor NGINX lagrer sitt standardoppsett.
Takk til  [@jarlefosen](https://github.com/jarlefosen) som foreslo løsningen. Merk at Vagrantfilen som er commit'et her bruker Ubuntu 14.04, som IKKE er nyeste Ubuntu.
