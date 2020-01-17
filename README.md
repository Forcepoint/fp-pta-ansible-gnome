# gnome

Install the GNOME Desktop.

If you intend to use this setup with Jenkins, you'll need to use the JNLP agent instead of the SSH agent because
any connections made via SSH come from the Jenkins master over SSH which won't 
get an environment which has access to the GUI. The only viable solution is to use a Jenkins JNLP agent started from 
within a user logged in to the OS via the GUI. If you use the jenkins-node-jnlp role, you'll get just that.

## Requirements

None

## Role Variables

None

## Dependencies

None

## Example Playbook

    - hosts: servers
      roles:
      - role: gnome

## License

BSD

## Author Information

Jeremy Cornett <jeremy.cornett@forcepoint.com>
