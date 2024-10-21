# Kalice :wine_glass:

*Kalice* is an [Ansible](https://www.ansible.com/) playbook to automate offensive Kali Linux configuration.

## TL;DR

Install `ansible` and run the playbook.

```bash
sudo apt install -y ansible
ansible-playbook main.yml
```

## RTFM

When executed, *Kalice* playbook will perform following operations.

- Set timezone.
- Update, upgrade and clean `apt` packages.
- Enable local firewall in `deny` mode, `auditd` and `lightdm`.
- Configure `vim` as default editor.
- Configure window manager appearance - *for `i3` usage only*.
- Download and install a multitude of offensive tools - *see [./roles/kalice/vars/main.yml]()*.

## License

See [LICENSE](./LICENSE) file.
