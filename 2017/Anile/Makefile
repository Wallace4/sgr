#
#		DNSmonitor
#   Copyright (C) 2017  Simone Anile simone.anile@gmail.com
#
#		This file is part of DNSmonitor.
#
#   DNSmonitor is free software: you can redistribute it and/or modify
#   it under the terms of the GNU General Public License as published by
#   the Free Software Foundation, either version 3 of the License, or
#   (at your option) any later version.
#
#   DNSmonitor is distributed in the hope that it will be useful,
#   but WITHOUT ANY WARRANTY; without even the implied warranty of
#   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
#   GNU General Public License for more details.
#
#   You should have received a copy of the GNU General Public License
#   along with DNSmonitor.  If not, see <http://www.gnu.org/licenses/>.
#
PCAP_LIB=-lpcap
THREAD_LIB=-lpthread
LIB=utils.c pagine.c

all: dnsa

PHONY: clean

dnsa: dnsa.c
	gcc dnsa.c -o dnsa $(LIB) $(PCAP_LIB) $(THREAD_LIB)

deb:
	gcc -g dnsa.c -o dnsa $(LIB) $(PCAP_LIB) $(THREAD_LIB) -Wall

clean:
	\rm -f *~ dnsa
