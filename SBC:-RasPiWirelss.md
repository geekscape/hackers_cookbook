# Summary
Add a new Wirelss access point using WPA security
# Usage

1. Make sure wpa_suplicant is installed

``sudo apt-get update && sudo apt-get install wpa_suplicant``

2. Run the command

``wpa_passphrase SSID WPA | sudo tee -a /etc/wpa_suplicant/wpa_suplicant.conf``

# References

<a rel="license" href="http://creativecommons.org/licenses/by-nc/3.0/deed.en_US"><img alt="Creative Commons License" style="border-width:0" src="http://i.creativecommons.org/l/by-nc/3.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" href="http://purl.org/dc/dcmitype/Text" property="dct:title" rel="dct:type">OSHCB</span> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc/3.0/deed.en_US">Creative Commons Attribution-NonCommercial 3.0 Unported License</a>.
