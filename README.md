# ubuntu-config

This playbook documents the configuration of my Ubuntu laptop(s) I use for school.

**Warning:** The `gnome` role will change your DE appearance!

## Execution instructions

    # Install ansible using your favorite method (mine is using pip)
    pip3 install ansible

    # clone this repository to your preferred location
    git clone https://github.com/casenull/ubuntu-config.git
    cd ubuntu-config

    # install the prerequisites
    ansible-galaxy collection install -r requirements.yml

    # run the playbook as a user with sudo rights
    ansible-playbook main.yml -K

## Additional information

This playbook can also be run using the tags `apt`,`gnome`,`docker`, `etc.`
(consult main.yml) to run only specific routines:

    # Run the Wireshark installation routine individually
    ansible-playbook main.yml -K --tags wireshark
