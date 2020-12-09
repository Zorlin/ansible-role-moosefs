Ansible Role: MooseFS
=====================

NOT READY FOR CONSUMPTION YET

This role will automatically build and install MooseFS from source.

It currently will only support Ubuntu 18.04 and Ubuntu 20.04 as I need this to maintain my own cluster.

I plan on changing that very soon however...

Planned support is for:

* CentOS 7, 8

* Debian 9, Debian 10

* Ubuntu 16.04, Ubuntu 18.04, Ubuntu 20.04

Goals:

* Use the best available (most supported, most stable) install method for each version and architecture combo. More on that later...

* Sane defaults but tunable knobs for all the things you may reasonably want to tune

Major planned features:

* Install from packages instead of building and installing MooseFS (I'm focusing on builds first as I'm using weird ARM boxes)

* Install from backports where available instead of using PPAs (Debian 9, Debian 10)

* A support set of playbooks that helps automate common tasks like upgrading master, metaloggers, chunkservers etc safely

* Support for amd64, arm32, arm64 architectures (I run a mix of all 3 in my personal MooseFS cluster). Special added stuff for ODROID HC2 and Helios64.

* GitHub Actions CI testing of tags to make sure they're good to go before release - for every supported platform

* Changelogs that let you track exactly what changed with each new tagged release

* Anything needed to automate building an Elastic NAS with this stuff

Stretch goal features:

* (MAYBE) Optional feature to enable jumbo frames if there's a nice safe way to do it

* (MAYBE) Wireguard stuff for transparent encryption between MooseFS components

Development of this role is driven primarily by the Elastic NAS I run at home, which uses MooseFS to make a really nice reliable NAS.

You can read all about it at https://raptorswithhats.com/tags/elasticnas/ - my blog with no ads or tracking.

New release versions of this role will be released when ready, using Semantic Versioning to keep things predictable.

I will not be changing or deleting release tags once published, so you can pin and rely on them safely.

If a critical fix is needed a new tag will be created :)

You should not rely solely on this stuff especially in production until I start publishing the 1.x.x series at least.

However, I will keep it as stable and production ready as possible.

Requirements
------------

Nothing yet.

Role Variables
--------------

Available variables are listed below, along with default values (see `defaults/main.yml`):

    NOT DOCUMENTED/IMPLEMENTED YET

Dependencies
------------

None.

Example Playbook
----------------

NOT DOCUMENTED/IMPLEMENTED YET

License
-------

MIT

Author Information
------------------

This role was created in 2020 by Benjamin Arntzen.

This role uses examples and code from [geerlingguy.awx](https://github.com/geerlingguy/ansible-role-awx) which was written by Jeff Geerling and is available under the MIT license.
