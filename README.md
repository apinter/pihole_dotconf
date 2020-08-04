<img src="https://raw.githubusercontent.com/apinter/pihole_dotconf/master/Screenshot.png">


# pihole_dotconf   
Configuration for PiHole DNS server v.5 and up.   
   
## Usage    
Install PiHole: https://github.com/pi-hole/pi-hole/#one-step-automated-install   
The `pi-hole-v5-teleporter.tar.gz` is the teleporter backup from PiHole, can be used to restore the lists at will from `PiHole wUI > Settings > Teleporter`.   
Included the lists though under their respective directory that can also be used. For adding domains to the whitelist I used this: https://github.com/anudeepND/whitelist. A little modification to the script whitelist.sh can pull down the whitelist included in this repo and apply it easily.
   
## Bulk whitelisting
To add multiple custom domains automatically to PiHole whitelist change the script from anudeepND's repo. Go to the [whitelist script](https://raw.githubusercontent.com/anudeepND/whitelist/master/scripts/whitelist.sh) and look for the line where it curl the whitelist.txt, looks like this: `curl -sS https://raw.githubusercontent.com/anudeepND/whitelist/master/domains/whitelist.txt` and change the URL to the whitelist you want to use.   
   
## Known issues   
* Whitelist is far from being complete.
