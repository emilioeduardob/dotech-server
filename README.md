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

```bash
ansible-playbook server-playbook.yml
```
