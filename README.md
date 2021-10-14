# Example playbook and report for ESXi information

This is an example playbook for pulling and reporting information from ESXi hosts.  You will need to populate the variables below in Tower.  Using other modules found in the [community.vmware](https://github.com/ansible-collections/community.vmware) collection you should be able to make this more dynamic.

## Required variables in tower
### Email Settings
- EMAIL_HOST - The email server being used to send report.
- EMAIL_PORT - The port to connect to on the email server.
- EMAIL_USERNAME - Username for email authentication
- EMAIL_PASSWORD - Password for email authentication
- EMAIL_FROM - The address that is sending the email.
- EMAIL_TO - The address you would like to recieve the email.
- EMAIL_SUBJECT - The subject of the email.

### VMWare Settings
- esxi_user - User that has access to the ESXi host.
- esxi_password - Password for the user that has access to the ESXi host.
- esxi_servers - Array of servers that you want to query.
