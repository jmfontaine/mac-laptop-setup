1. Install Ansible.

- Run the following command to add Python 3 to your $PATH: `export PATH="$HOME/Library/Python/3.8/bin:/opt/homebrew/bin:$PATH"`

- Upgrade Pip: `sudo pip3 install --upgrade pip`

- Install Ansible: `pip3 install ansible`

2. Clone or download this repository to your local drive.
3. Run `ansible-galaxy install -r requirements.yml` inside this directory to install required Ansible roles.
4. Run `ansible-playbook --ask-become-pass playbook.yml` inside this directory. Run `ansible-playbook --ask-become-pass --tags "dotfiles,homebrew" playbook.yml` to only run the tasks associated with those tags.
