# exp-7
---
- name: Basic Server Setup
hosts: localhost
become: yes # Use privilege escalation (sudo)

tasks:
- name: Update apt cache
apt:
update_cache: yes

- name: Install curl
apt:
name: curl
state: present
