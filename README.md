<p align="center"><img src="images/kalice.png" width="256" height="256" alt="Kalice"></p>
<h1 align="center">Kalice</h1>
<p align="center">Ansible playbook to automate offensive Kali Linux configuration</p>
<hr>

## TL;DR

Install [Ansible](https://docs.ansible.com/) then run the playbook.

```bash
sudo apt update -y
sudo apt install -y ansible
ansible-playbook main.yml
```

## RTFM

When executed, *Kalice* playbook will perform following operations.

* Update, upgrade and clean `apt` packages.
* Set timezone.
* Enable `auditd`.
* Configure [vim](https://www.vim.org/) as default editor.
* Download and install a multitude of offensive tools - *see [./roles/kalice/vars/main.yml](./roles/kalice/vars/main.yml)*.
* Clean useless files.

## License

See [LICENSE](./LICENSE.txt) file.
