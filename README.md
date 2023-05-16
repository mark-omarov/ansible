# Mark's Development Environment Ansible Playbook

This is a playbook to set up my development environment on a new machine. It's a work in progress, and I'm not sure how useful it will be to anyone else. I'm using it to document and automate my own setup.

## Ansible Installation

0. Install [Homebrew][homebrew]
1. Install [pyenv][pyenv]
2. Install Python - `pyenv install 3.11.1`
3. Install Ansible - `pip install ansible`

## Running the Playbook

0. Install [mas][mas].
1. Clone this repository
2. Install ansible galaxy dependencies - `ansible-galaxy install -r requirements.yml`
3. Run the playbook - `ansible-playbook main.yml --ask-become-pass --ask-vault-pass`

## Credentials

Big shout out to [Jeff Geerling][geerlingguy] for his [Mac Collection for Ansible][ansible-for-mac] collection and [Elliot Weiser][elliotweiser] for his [osx-command-line-tools][ansible-osx-clt] Ansible role.

I used products they created to avoid lots of manual work. I also used their documentation as a reference for how to do things.

[homebrew]: https://brew.sh/
[pyenv]: https://github.com/pyenv/pyenv
[firefoxde]: https://www.mozilla.org/en-US/firefox/developer/
[raycast]: https://raycast.com/
[ansible-vault]: https://docs.ansible.com/ansible/latest/vault_guide/index.html
[mas]: https://github.com/mas-cli/mas
[geerlingguy]: https://github.com/geerlingguy
[ansible-for-mac]: https://github.com/geerlingguy/ansible-collection-mac/
[elliotweiser]: https://github.com/elliotweiser
[ansible-osx-clt]: https://github.com/elliotweiser/ansible-osx-command-line-tools
