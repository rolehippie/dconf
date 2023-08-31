# dconf

[![Source Code](https://img.shields.io/badge/github-source%20code-blue?logo=github&logoColor=white)](https://github.com/rolehippie/dconf)
[![General Workflow](https://github.com/rolehippie/dconf/actions/workflows/general.yml/badge.svg)](https://github.com/rolehippie/dconf/actions/workflows/general.yml)
[![Readme Workflow](https://github.com/rolehippie/dconf/actions/workflows/docs.yml/badge.svg)](https://github.com/rolehippie/dconf/actions/workflows/docs.yml)
[![Galaxy Workflow](https://github.com/rolehippie/dconf/actions/workflows/galaxy.yml/badge.svg)](https://github.com/rolehippie/dconf/actions/workflows/galaxy.yml)
[![License: Apache-2.0](https://img.shields.io/github/license/rolehippie/dconf)](https://github.com/rolehippie/dconf/blob/master/LICENSE)
[![Ansible Role](https://img.shields.io/badge/role-rolehippie.dconf-blue)](https://galaxy.ansible.com/rolehippie/dconf)

Ansible role to configure global dconf profiles.

## Sponsor

Building and improving this Ansible role have been sponsored by my current and previous employers like **[Cloudpunks GmbH](https://cloudpunks.de)** and **[Proact Deutschland GmbH](https://www.proact.eu)**.

## Table of content

- [Requirements](#requirements)
- [Default Variables](#default-variables)
  - [dconf_default_profiles](#dconf_default_profiles)
  - [dconf_extra_profiles](#dconf_extra_profiles)
- [Discovered Tags](#discovered-tags)
- [Dependencies](#dependencies)
- [License](#license)
- [Author](#author)

---

## Requirements

- Minimum Ansible version: `2.10`

## Default Variables

### dconf_default_profiles

#### Default value

```YAML
dconf_default_profiles:
  - name: gdm
    profile: |
      user-db:user
      system-db:gdm
      file-db:/usr/share/gdm/greeter-dconf-defaults
    configs:
      - name: login-screen
        config: |
          [org/gnome/login-screen]
          disable-user-list=true
```

### dconf_extra_profiles

#### Default value

```YAML
dconf_extra_profiles: []
```

## Discovered Tags

**_dconf_**


## Dependencies

- None

## License

Apache-2.0

## Author

[Thomas Boerger](https://github.com/tboerger)
