---
- hosts: all
  become: true
  roles:
    - update_packages
    - install_packages
    - create_samba_credentials
    - add_samba_share_into_fstab
    - remount_fstab_mounts

  vars:
    packages:
      - avahi-daemon
      - cifs-utils
      - psmisc
      - samba
      - samba-common
      - smbclient
      - wsdd

    samba_share:
      server: "smb.example.com"
      share_path: "/shared"
      mount_point: "/mnt/shared"

    samba_credentials:
      file: "/etc/samba/{{ ansible_hostname }}.smbclient"
      username: "your_username"
      password: "your_password"
      domain: "WORKGROUP"
