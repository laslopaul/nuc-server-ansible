# nuc-server-ansible

Ansible configuration files for nuc-server

## Installation

1. Install ansible to the server

2. Save `zerotier_net_id` and `repo_token` for fluxcd repo to `/root/vars.yml`

3. Save Zerotier API token to `/var/lib/zerotier-one/token`

4. Run ansible-pull as root

```bash
cd /root
ansible-pull -U https://github.com/laslopaul/nuc-server-ansible -i hosts -e @vars.yml
```
