# gnome

Install the GNOME Desktop.

If you intend to use this setup with Jenkins, you'll need to use the JNLP agent instead of the SSH agent because
any connections made via SSH come from the Jenkins master over SSH which won't 
get an environment which has access to the GUI. The only viable solution is to use a Jenkins JNLP agent started from 
within a user logged in to the OS via the GUI. If you use the jenkins-node-jnlp role, you'll get just that.

## Requirements

As of this writing (2020-01-29), this role does not apply with the docker-host role as
you'll get a conflict with urllib3 being applied by pip and by yum.

## Role Variables

None

## Dependencies

None

## Example Playbook

    - hosts: servers
      roles:
      - role: gnome

## License

BSD-3-Clause

## Author Information

Jeremy Cornett <jeremy.cornett@forcepoint.com>
