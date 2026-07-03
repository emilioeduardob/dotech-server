# Dotech Playbooks

# Setup

## Requirements

Install Ansible 2.2.0 stable

## Hosts

Create `hosts` file and include your hosts

```yaml
[digitalocean]
104.236.101.195
```

## Dependencies

Install additional modules

```bash
ansible-galaxy install -r requirements.yml
```

## Running

By default the playbook connects as the `deploy` user. For the first run on a
fresh server, connect as `root` so the `deploy` user can be created:

```bash
ansible-playbook -u root server-playbook.yml
```

After the first run `root` SSH access is disabled, so use the `deploy` user:

```bash
ansible-playbook server-playbook.yml
```
