# iocage-plugin-template
Template file and directory structure for iocage plugins.

This repository defines the proposed structure of an iocage-based container.

Feedback appreciated.

Let's do this right!

-----

Contents of a container template repository.

- LICENSE: container license

- README: container README document

- overlay/: drop-in overlay files. (optional)

- plugin.json: Baseline container definitions:
  - name: container name
  - release: base FreeBSD version
  - pkg: list of ports/packages to be installed
  - pkgsite: valid pkg repository
  - fingerprints: poudriere repo trusted fingerprints

- post_install.ext: any post_install scripting (any supported .ext)
  - (could this be config-management-pluggable?)

- settings.json: JSON file which controls plugins settings interface

- ui.json: FreeNAS stuff
