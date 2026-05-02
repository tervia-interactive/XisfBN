XisfBN Source:
---------------
This is the top level of the XisfBN source directory.

XisfBN, short for "X is so fire, but new!", is an operating system and kernel project
based on FreeBSD, using the same general source tree architecture and file organization.

XisfBN is the continuation of the original Xisf kernel project, short for
"X is so fire!". The project keeps the FreeBSD-style layout while introducing
the XisfBN identity, custom kernel direction, and system-level changes.

XisfBN may also be referred to by its abbreviation: XbN.

FreeBSD is used as the base for XisfBN because of its mature kernel design,
portable source tree, networking stack, security features, storage support,
and long-standing UNIX-like architecture.

For copyright information, please see [the file COPYRIGHT](COPYRIGHT) in this
directory. Additional copyright information may also exist for some sources in
this tree - please see the specific source directories for more information.

The Makefile in this directory supports a number of targets for building
components, the kernel, userland, or the complete XisfBN source tree.

Because XisfBN is based on FreeBSD, some build documentation from FreeBSD may
still be useful as upstream reference material, including build(7), config(8),
the FreeBSD Handbook section on building userland, and the FreeBSD Handbook
section for kernel configuration.

For information on CPU architectures and platforms supported by the upstream
FreeBSD base, see the FreeBSD website's Platforms page:

https://www.freebsd.org/platforms/

XisfBN may support the same or a reduced set of architectures depending on the
current state of the XisfBN kernel and system source tree.

Source Roadmap:
---------------
| Directory | Description |
| --------- | ----------- |
| bin | System/user commands. |
| cddl | Various commands and libraries under the Common Development and Distribution License. |
| contrib | Packages contributed by third parties. |
| crypto | Cryptography-related source code and tools. See [crypto/README](crypto/README). |
| etc | Template files for /etc. |
| gnu | Commands and libraries under the GNU General Public License or Lesser General Public License. Please see [gnu/COPYING](gnu/COPYING) and [gnu/COPYING.LIB](gnu/COPYING.LIB) for more information. |
| include | System include files. |
| kerberos5 | Kerberos5 package. |
| lib | System libraries. |
| libexec | System daemons. |
| release | Release building Makefile and associated tools. |
| rescue | Build system for statically linked /rescue utilities. |
| sbin | System commands. |
| secure | Cryptographic libraries and commands. |
| share | Shared resources. |
| stand | Boot loader sources. |
| sys | XisfBN kernel sources. See [sys/README.md](sys/README.md). |
| targets | Support for experimental DIRDEPS_BUILD. |
| tests | Regression tests which can be run by Kyua. See [tests/README](tests/README) for additional information. |
| tools | Utilities for regression testing and miscellaneous tasks. |
| usr.bin | User commands. |
| usr.sbin | System administration commands. |

Project Notes:
---------------
XisfBN is not a separate-from-scratch layout. It follows the FreeBSD-style source
tree so that developers familiar with FreeBSD can understand and work with the
system more easily.

The main goals of XisfBN are:

- Continue the original Xisf kernel project.
- Keep compatibility with the FreeBSD-style architecture and source layout.
- Provide a custom identity under the XisfBN / XbN name.
- Allow kernel and system-level experimentation while keeping a familiar UNIX-like base.
- Build a modern continuation of "X is so fire!" under the new name:
  "X is so fire, but new!"

Upstream Base:
---------------
XisfBN is based on FreeBSD. Some files, tools, documentation references, and
directory structures may still come from or resemble FreeBSD.

When modifying XisfBN, check the license information in each directory before
redistributing changes.

Building:
---------------
The source tree can be built using the Makefile targets available in this
directory.

Typical build targets may include building userland, building the kernel, or
building a complete system image, depending on the current state of the XisfBN
tree.

For FreeBSD-compatible build behavior, refer to the upstream FreeBSD build
documentation as a reference.

Name:
---------------
Full name: XisfBN  
Meaning: X is so fire, but new!  
Abbreviation: XbN  
Previous project: Xisf  
Previous meaning: X is so fire!
