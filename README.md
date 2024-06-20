# funmilayo-warden-
warden
wget -q -O warden.sh https://api.nodes.guru/warden.sh && sudo chmod +x warden.sh && ./warden.sh && source $HOME/.bash_profile
wardend keys add wallet
wardend keys add wallet --recover
curl -XPOST -d '{"warden1dw0dsmqwx80593qvcc4lxtmsv2mm4we2nu9hfc": ""}' https://faucet.buenavista.wardenprotocol.org
wardend q bank balances $(wardend keys show wallet -a)
wardend tx staking create-validator $HOME/.warden/validator.json \
    --from=wallet \
    --chain-id=buenavista-1 \
    --fees=500uward -y
    
