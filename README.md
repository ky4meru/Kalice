# Kalice :wine_glass:

*Kalice* is an [Ansible](https://www.ansible.com/) playbook to automate offensive Kali Linux configuration.

## TL;DR

Install `ansible` then run the playbook.

```bash
sudo apt update -y
sudo apt install -y ansible
ansible-playbook main.yml
```

## RTFM

When executed, *Kalice* playbook will perform following operations.

- Update, upgrade and clean `apt` packages.
- Set timezone.
- Enable `auditd`.
- Configure `vim` as default editor.
- Download and install a multitude of offensive tools - *see [./roles/kalice/vars/main.yml](./roles/kalice/vars/main.yml)*.

## License

See [LICENSE](./LICENSE) file.
