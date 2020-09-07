# Yandex Cloud OpenVPN server 

1. install Ansible

2. run

```bash
ansible-playbook provision.yml
```

3. type openvpn user password on prompt

4. run

```bash
sudo openvpn --config data/vpnuser.ovpn
```

5. open `http://ip.yandex.ru/` to make sure you looks like russian

6. to get back, just run

```bash
ansible-playbook remove.yml
```