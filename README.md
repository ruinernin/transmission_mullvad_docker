# transmission_mullvad_docker
Transmission client behind Mullvad (wireguard) in containers

## Setup Mullvad & wireguard
Generate a config and new keys through the mullvad web UI and choose an
enpoint (City) close to you to use. Then open a port for your new key in the UI
under 'Port forwarding'. Select the city you're going to connect to then the ID
of the key you're going to use and add a port, note down the port that was
opened for you `cc-cit-XXXXX` where `XXXXX` will be the port opened.

Edit `wg.conf` so it has all the needful.

## Setup transmission
Once you've got the containers up use the transmission web UI to set your open
port to the one that was generated previously. Use the 'test' button to check
it works.
