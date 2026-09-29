# Проект: Безопасность GNU/Linux, РЕД ОС 8 (номер 372311)

| Пункт | Что сделано | Команды |
|---|---|---|
| 1.1–1.3 | DHCP, hostname, ping | nmcli, hostnamectl, ping |
| 2 | Обновление, nginx, libcap-ng-utils, tcpdump | dnf, dnf download, rpm -ivh |
| 3 | Раздел sdb1, ext4, метка MEPHI_WEB, fstab | fdisk, mkfs.ext4 -L, mount |
| 4 | nginx enable --now, journalctl | systemctl, journalctl |
| 5.1 | Группы, ACL, setgid | groupadd, useradd, setfacl |
| 5.2 | Capabilities вместо SUID | setcap cap_net_raw,cap_net_admin=eip |
| 5.3 | SELinux Enforcing, httpd_sys_content_t | semanage fcontext, restorecon |
| 6.1 | Запрет входа curators | pam_succeed_if в /etc/pam.d/login |
| 6.2 | 90 дней, minlen=12 | login.defs, pwquality.conf, chage |
| 7 | index.html, curl | echo, curl http://localhost/ |
