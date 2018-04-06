# Ansible role 'ansible-role-fish'

An Ansible role for setting up fish shell and oh-my-fish.
If you do not wish for oh-my-fish to be installed, a simple override file can be created on the remote node prior to running:
```sh
sudo touch /etc/omf.installed
```

## Requirements
- Git installed on the node.
- Any distribution which the `package` module supports, and a repo installed where `fish` exists with that exact name.

## Role Variables
| Variable		| Default		| Comments (type) |
| :---			| :---			| :---		  |
|`userlist` | | Dictionary containing of base directory (for home dirs)(value) and username (key)|
## Dependencies

## Example Playbook
```Yaml
- hosts: foo
  roles:
    - role: ansible-role-fish
      userlist:
        foouser: /home/
```

## Testing


## License

BSD

## Contributors

Issues, feature requests, ideas, suggestions, etc. are appreciated and can be posted in the Issues section. Pull requests are also very welcome. Please create a topic branch for your proposed changes, it's the easiest way to merge back into the project.

- [Oscar Petersson](https://github.com/oscpe262/) (Maintainer)
