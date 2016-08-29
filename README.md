deekayen-macbook ansible playbook
=================================

Install Homebrew
----------------

[Some people make a complicated Ansible role for this](https://github.com/geerlingguy/ansible-role-homebrew/network), but I'm only doing it once, so just run the install command from http://brew.sh/ in Terminal!

Install Ansible
---------------

According to the [Ansible installation docs](
https://docs.ansible.com/ansible/intro_installation.html#latest-releases-via-pip), the preferred way to install for macOS is via pip, however I never got it to install with the recommended process and upgrade cleanly between versions. The Homebrew-installed ansible package works better for me.

```
brew install ansible
```

Clone this Repo
---------------

Yeah, just do that.

Run the playbook
----------------

Ansible makes setup easy. This playbook is intended to run all its tasks as local actions, so an inventory file is not necessary.

```
ansible-playbook main.yml
```

TODO
----

Add default colors for iTerm:
https://github.com/stephenway/monokai.terminal

Add default config and packages for Sublime (e.g.):
https://packagecontrol.io/packages/Base16%20Color%20Schemes

Add Adobe Source font series (e.g.):
https://github.com/adobe-fonts/source-code-pro
