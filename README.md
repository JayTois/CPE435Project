# CPE435Project

This is used to harden servers for CPE435.
- The servers are hardened using the Ansible scripting language.
- More documentation is included in each of the YAML files

cronjobs.yml
- Gets rid of any unwanted cronjobs that could cause vulnerabilities

main.yml
- Calls all of the ansible playbooks

permchange.yml
- Takes important files and changes the permissions and makes them immutable with 'chattr'

rootlock.yml
  - prevents password login via root

ufw.yml - uncomplicated firewasll
- allows and prevents different ports (servivces)
- restarts the firewall subsequently to update services

update.yml
- updates important packages (made for ubuntu)
- includes other important packages for users such as nano, htop, etc.


