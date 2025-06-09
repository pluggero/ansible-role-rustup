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

```yaml
rustup_install_method: "dynamic"
```

The method used to install rustup can be defined in the variable `rustup_install_method`.
The following methods are available:

- `source`: Installs rustup from source
- `package`: Installs rustup from the package manager of the distribution
  - **NOTE**: This method installs the latest version available in the package manager and not the version defined in `rustup_version`.
- `dynamic`: Installs rustup from package manager if available in the correct version, otherwise installs from source

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
