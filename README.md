- name: Install and configure Samba server
  hosts: 1C-servers
  become: yes

  roles:
  - role: 1c_postgres
  #  when: ansible_lsb.codename == 'focal'
  # - role: common
  #   when: ansible_lsb.codename == 'focal'
  # - role: builder
  #   when: ansible_lsb.codename == 'focal'
  # - role: prod
