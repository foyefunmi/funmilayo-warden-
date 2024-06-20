# funmilayo-warden-
warden
wget -q -O warden.sh https://api.nodes.guru/warden.sh && sudo chmod +x warden.sh && ./warden.sh && source $HOME/.bash_profile
wardend keys add wallet
wardend keys add wallet --recover
curl -XPOST -d '{"address": "YOUR_WALLET_ADDRESS"}' https://faucet.buenavista.wardenprotocol.org
wardend q bank balances $(wardend keys show wallet -a)
