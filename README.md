# Yandex Cloud OpenVPN server 

1. Yandex Cloud CLI

Check for `ya` util existst.

If none, install it:

```bash
curl https://storage.yandexcloud.net/yandexcloud-yc/install.sh | bash
```
Follow the instructions of installer.

Initialize it by executing `yc init`.

2. install Ansible

3. run

```bash
ansible-playbook provision.yml
```

4. type openvpn user password on prompt

5. run

```bash
sudo openvpn --config data/vpnuser.ovpn
```

6. open `http://ip.yandex.ru/` to make sure you looks like russian

7. to get back, just run

```bash
ansible-playbook remove.yml
```
