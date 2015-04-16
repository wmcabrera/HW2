ANALYZING PACKET SNIFFING  DATA

Wellington Cabrera


1. How to run:

Please execute tt the shell prompt the script  in this way : ./analyze filename.
The script is programmed in AWK

File name should be a package capture file, in format csv.

2. How to convert .dmp or .pcap to csv

Open your .dmp or .pcap file using WirShark. Then choose the option
"Export packages Disecctions" -> as CSV


3. Output

TOP Source Address : Shows the Address/Name of source hosts ( > 5%)
TOP Destination Address:Shows the Address/Name of destination hosts ( > 5%)
TOP Protocols: Protocolsthat show up at least 5%
TCP Duplic ACK: Counting of Duplicate ACKs
TCP Retransmiss: Counting of TCP Retransmissions
TOTAL PACKAGES: Total of Packages


SAMPLE OUTPUT

TOTAL PACKAGES 555218 


TOP Source Addr: #PCK   %
---------------------------
"129.7.243.106" 31216 5.6223%
"129.7.243.241" 240735 43.3586%
"73.32.37.242" 34924 6.29014%

TOP Destin Addr: #PCK   %
---------------------------
"broadcast" 36752 6.61938%
"129.7.243.241" 104021 18.7352%
"224.0.0.251" 31094 5.60032%
"129.7.243.255" 53269 9.59425%
"73.32.37.242" 160935 28.9859%

TOP Protocols  : #PCK   %
---------------------------
"tcp" 171128 30.8218%
"arp" 36934 6.65216%
"sshv2" 163744 29.4918%
"llmnr" 32880 5.922%
"mdns" 49952 8.99683%
"nbns" 33244 5.98756%


TCP Duplic  ACK PCK: 11553 2.0808%
TCP Retransmiss PCK: 62690 11.2911%

