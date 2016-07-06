# mac-address-last-octets
=======

Overview
--------
Wordlist of all possible last 3 octets of MAC address NIC identifiers.

Use with any WPA wordlist cracker. I made this to crack Wifi routers which some ISP's set up using the MAC address as the password, and sometimes, merely 1-up the last number.

Prepend the router's OUI (first 3 octets) with sed.

For instance, to crack BEC routers using OUI 600347:
sed -e 's/^/600347/' last_octets_mac_addresses.txt > bec_router_wordlist.txt

Author
--------
@rare1teas
