__ YUM:  
On Red Hat Enterprise Linux 8, installing software is ensured by the new version of the YUM tool, which is based on the DNF technology (YUM v4).  
Usage of YUM has not been changed when handling individual RPM packages. For handling the modular content, the yum module command has been added


__ RHEL 8 Module:
A module is a set of RPM packages that represent a component and are usually installed together. A typical module contains packages with an application, packages with the application-specific dependency libraries, packages with documentation for the application, and packages with helper utilities.


__ Application streams:



Python 3.6 is the default Python implementation in RHEL 8


__ Wayland:
The GNOME session and the GNOME Display Manager use Wayland as their default display server.
The X.Org server, which is the default display server in RHEL 7, is available as well.

__ DBs:
The following database servers are distributed with RHEL 8: MariaDB 10.3, MySQL 8.0, PostgreSQL 10, PostgreSQL 9.6, and Redis 5

__ Webservers:
RHEL 8 provides the Apache HTTP Server 2.4 and introduces a new web server, nginx 1.14.

__ LEAPP:
Upgrade from RHEL 7 to RHEL 8 -> Leapp

The nftables framework replaces iptables in the role of the default network packet filtering facility.
The firewalld daemon now uses nftables as its default backend.


— File Systems and Storage
The XFS file system now supports shared copy-on-write data extend functionality that allows sharing a common set of data blocks. It means everyone has a single shared copy of the file that links the same data blocks. This functionality allows minimizing the number of data blocks.

_ Stratis is now available

Stratis is a new local storage manager. It provides managed file systems on top of pools of storage with additional features to the user.

Stratis enables you to more easily perform storage tasks such as:

Manage snapshots and thin provisioning
Automatically grow file system sizes as needed
Maintain file systems
To administer Stratis storage, use the stratis utility, which communicates with the stratisd background service.

Stratis is provided as a Technology Preview.

Docker is not included in RHEL 8.0. For working with containers, use the podman, buildah, skopeo, and runc tools.
The podman tool has been released as a fully supported feature.

The podman tool manages pods, container images, and containers on a single node. It is built on the libpod library, which enables management of containers and groups of containers, called pods.

Virtual machines can now be created and managed using the RHEL 8 web console, also known as Cockpit.


