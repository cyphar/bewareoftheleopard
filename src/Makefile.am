# remainroot: a shim to trick code to run in a rootless container
# Copyright (C) 2016 Aleksa Sarai <asarai@suse.de>
#
# remainroot is free software: you can redistribute it and/or modify
# it under the terms of the GNU General Public License as published by
# the Free Software Foundation, either version 3 of the License, or
# (at your option) any later version.
#
# remainroot is distributed in the hope that it will be useful,
# but WITHOUT ANY WARRANTY; without even the implied warranty of
# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
# GNU General Public License for more details.
#
# You should have received a copy of the GNU General Public License
# along with remainroot.  If not, see <http://www.gnu.org/licenses/>.

# remainroot
bin_PROGRAMS = remainroot
remainroot_SOURCES = remainroot.c core/cred.c core/proc.c
noinst_HEADERS = common.h info.h shims.h core/cred.h core/proc.h core/syscalls-def.h core/syscalls-undef.h

# ptrace shim
remainroot_SOURCES += ptrace.c ptrace/generic-shims.c ptrace/amd64.c ohmic/ohmic.c
noinst_HEADERS += ptrace/generic.h ptrace/generic-shims.h ohmic/ohmic.h
