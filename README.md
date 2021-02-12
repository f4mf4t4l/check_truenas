# check_truenas
Check Plugin for truenas 2.0 API

## Install dependencies:

(apt/yum/dnf) install python3

pip3 install requests click humanfriendly NagiosCheckHelper

## Create API Key

From the Manual: https://www.truenas.com/docs/hub/additional-topics/api/

To create an API key, open the web interface (Settings - Gear Icon) menu and click "API KEY".
Name the API key something like "Nagios Access"


## Examples:

check_truenas -t token_here -H 192.168.168.210 pool -w 82 -c 92

check_truenas -t token_here -H 192.168.168.210 replications

check_truenas -t token_here -H 192.168.168.210 alerts

check_truenas -t token_here -H 192.168.168.210 updates

