# debian-system-update
This is a simple Ansible-based Action to update a Debian system I created to practice CI/CD pipelines.


## Usage
To use this template, you'll need to provide several secrets:
1. A valid SSH key for Ansible to use to connect to target systems (`{{ SSH_PRIVATE_KEY }}`)
2. A sudo password for elevated privledges, if needed. If not - you'll need to set `become` to `no` in `update-debian-system.yaml`
3. An Ansible inventory file. I'm cloning it from another repository via an access token - you can do the same or simply provide it.
