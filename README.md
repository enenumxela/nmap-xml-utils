# nmap-xml-utils

Utilities to process nmap XML output.

## Scripts

* [Merge nmap xml files](#merge-nmap-xml-files)
* [Parse nmap xml file](#parse-nmap-xml-file)

### [Merge nmap xml files](https://raw.githubusercontent.com/enenumxela/nmap-xml-utils/main/nmap-xml-merge.py)

Merge Multiple nmap xml output files into a single xml file.

#### Installation

```bash
curl -sL https://raw.githubusercontent.com/enenumxela/nmap-xml-utils/main/nmap-xml-merge.py > ~/.local/bin/nmap-xml-merge.py && chmod u+x ~/.local/bin/nmap-xml-merge.py
```

#### Uage

```bash
nmap-xml-merge.py -h
```

```text
usage: nmap-xml-merge [-h] [-f FILE] [-d DIR] [-q]

optional arguments:
  -h, --help            show this help message and exit
  -f FILE, --file FILE  parse FILE
  -d DIR, --dir DIR     Parse all xml in directory
  -q, --quiet           don't print status messages to stdout
```

### [Parse nmap xml file](https://raw.githubusercontent.com/enenumxela/nmap-xml-utils/main/nmap-xml-parse.py)

Parse nmap xml output file to extract bits of information.

#### Installation

```bash
curl -sL https://raw.githubusercontent.com/enenumxela/nmap-xml-utils/main/nmap-xml-parse.py > ~/.local/bin/nmap-xml-parse.py && chmod u+x ~/.local/bin/nmap-xml-parse.py
```

#### Uage

```bash
nmap-xml-parse.py -h
```

```text
usage: nmap-xml-parse [-h] [-ips] [-ports] [-service SERVICE] [-service-prefix PREFIX] [-separator SEPARATOR] FILE

positional arguments:
  FILE                  Nmap XML output file

optional arguments:
  -h, --help            show this help message and exit
  -ips                  list of live ipv4s
  -ports                list open ports
  -service SERVICE      service to filter by
  -service-prefix PREFIX
                        service prefix to filter by
  -separator SEPARATOR  output separator
```