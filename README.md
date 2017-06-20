This MACsec key chain Ansible playbook is focused on simplifying the re-key process for customers using MACsec with pre-shared keys, running Cisco router platforms that run IOS-XE, and have the hardware capable of supporting the new WAN MACsec capabilities.  Customers leveraging MACsec (or any encryption solution using pre-shared keys) know, changing keys can be a rigorous repeatable process, to the point keys remain in place much longer than they should.  Leveraging this Ansible playbook for MACsec key chain modification, will offer operators the ability to automate the MACsec key chain configuration through Ansible playbooks.

Cisco IOS-XE documentation for configuring MACsec can be found at:  http://www.cisco.com/c/en/us/td/docs/ios-xml/ios/macsec/configuration/xe-3s/macsec-xe-3s-book.html

Comments to users of this playbook.  Like any automation methods, there are multiple ways to target solving the problem.  While I typically try to leverage templates (Jinja2) as much as possible, this configuration in IOS-XE is relatively flat, so while I used a variables file, an operator can choose to break up this IOS-XE configuration in the IOS Module as much as you desire.  The playbook here modularizes the playbook into the major categories needed, but how much the playbook is broken up, is up to the operator.
