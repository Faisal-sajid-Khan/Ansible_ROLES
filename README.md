# Ansible_ROLES
Ansible_ROLES
# Ansible Role: Apache2 (httpd) Installation & File Management

This is my **first Ansible Galaxy role**.  
It installs **Apache2 (httpd)** on Ubuntu and manages files (copying from terminal with owner, group, and permission settings).

---

## 🚀 Features
- Installs **Apache2 (httpd)** on Ubuntu.
- Copies files from local terminal to the server.
- Sets **owner, group, and permissions** for copied files.
- Works with Ansible Galaxy role structure.

---

## 📋 Requirements
- Ansible >= 2.9  
- Ubuntu (tested on 20.04/22.04)  
- Sudo/root privileges  

---

## ⚙️ Role Variables
You can customize the following variables in `defaults/main.yml`:

```yaml
apache_package: apache2     # Package name for Apache
file_src: /path/to/local/file
file_dest: /var/www/html/index.html
file_owner: www-data
file_group: www-data
file_mode: '0644'
