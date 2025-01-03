# Ansible Role: Rustup and Rust toolchain

[![CI](https://github.com/pluggero/ansible-role-rustup/actions/workflows/ci.yml/badge.svg)](https://github.com/pluggero/ansible-role-rustup/actions/workflows/ci.yml) [![Ansible Galaxy downloads](https://img.shields.io/ansible/role/d/pluggero/rustup?label=Galaxy%20downloads&logo=ansible&color=%23096598)](https://galaxy.ansible.com/ui/standalone/roles/pluggero/rustup)

An Ansible Role that installs Rustup and Rust toolchain.

## Requirements

None.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

```yaml
rustup_rust_version: "<version>"
```

The default version of Rust to install.

## Dependencies

None.

## Example Playbook

```yaml
- hosts: all
  roles:
    - pluggero.rustup
```

## License

MIT / BSD

## Author Information

This role was created in 2025 by Robin Plugge.
