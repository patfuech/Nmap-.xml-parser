With this setup, you must specify the ports every time you run the script, but the directory and output file name have default values which you can override manually within the script.

To run the script, navigate to the directory where it's located (or add its location to your PATH), and use a command like:

`python ~/Tools/port_scan_parser.py --ports 22 80`

This command will scan for open ports 22 and 80 in the default directory (~/def_cred_scan/Blomberg) and output the results to files ip_addresses_22.txt and ip_addresses_80.txt in the current directory.

If you want to specify a different directory or output file base name, you can do so:

`python ~/Tools/port_scan_parser.py -p, --ports 161 -o, --output ip_results path/to/.xml_files/to/parse/`

This would search /mnt/smb/Depts/Proactive Services/threat Hunting/IPT/" for open port 161 and output to ip_results_161.txt in the current working directory.
