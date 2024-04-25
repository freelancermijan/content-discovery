# content_discovery_for_all_in_one
# collected from researchers

## Sample

```
cgi-bin/dmt/reset.cgi?db_prefix=%26id%26
cgi-bin/reset.cgi?db_prefix=%26id%26
cgi-bin/FUZZ.cgi?FUZZ=%26id%26
```
## Installations

```
sudo mkdir -p /usr/share/wordlists/
cd /usr/share/wordlists/
sudo git clone https://github.com/freelancermijan/content-discovery.git
cd
```

## Updating

```
cd /usr/share/wordlists/content-discovery/
sudo git pull
cd
```

## Usage

```
ffuf -u http://testphp.vulnweb.com/FUZZ -w /usr/share/wordlists/content-discovery/content_discovery_for_all.txt -v -c -fs 0 -fc 404,500 -mc 200 -recursion -o ffuf_scan_result.txt  
```
