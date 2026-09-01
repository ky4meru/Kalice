<p align="center"><img src="images/kalice.png" width="256" height="256" alt="Kalice"></p>
<h1 align="center">Kalice</h1>
<p align="center">Ansible playbook to automate offensive Kali Linux configuration</p>
<hr>

# Usage

> [!IMPORTANT]
> It is strongly recommended to reboot the host after playbook execution.

## Prerequisites

Install [Ansible](https://docs.ansible.com/) and the required collections.

```bash
sudo apt update -y
sudo apt install -y ansible
ansible-galaxy collection install -r requirements.yml
```

## Run locally

As simple as that.

```bash
ANSIBLE_CONFIG=ansible.cfg ansible-playbook main.yml --ask-become-pass
```

## Run remotely

Add your remote hosts to [inventory/hosts.yml](./inventory/hosts.yml).

```yaml
kalice:
  hosts:
    localhost:
      ansible_connection: local
    kali-linux:
      ansible_host: 10.10.0.42
      ansible_user: kali
```

Then restrict the run to that hosts.

```bash
ANSIBLE_CONFIG=ansible.cfg ansible-playbook main.yml --limit kali-linux --ask-become-pass
```

# License

See [LICENSE](./LICENSE.txt) file.
