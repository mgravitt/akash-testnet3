
# Stake to Validator
akash tx staking delegate akashvaloper19zu8ydx5q90vs3j5993aukne7a7mdw9d978gfk 5000uakt --from akash145kmcq2zuqlrzj6raa9p86ukjclsp7prr59x0y --fees 5000uakt

# Vote on proposal
akash tx gov vote 3 yes --from akash145kmcq2zuqlrzj6raa9p86ukjclsp7prr59x0y --fees 5000uakt

# Authorize a send
akash tx authz grant akash1jq42qysz9tnwa7my645qt2eg4gm8fgn39pmxtr send --spend-limit=50akt --from akash145kmcq2zuqlrzj6raa9p86ukjclsp7prr59x0y  --fees 5000uakt

# Authorize a generic message type
akash tx authz grant akash145kmcq2zuqlrzj6raa9p86ukjclsp7prr59x0y generic --msg-type=/akash.deployment.v1beta2.MsgCreateDeployment --from akash1jq42qysz9tnwa7my645qt2eg4gm8fgn39pmxtr --fees 5000uakt


/akash.market.v1beta2.MsgCreateLease
/akash.deployment.v1beta2.MsgCreateDeployment

# Create a market lease
akash tx market lease create --chain-id $AKASH_CHAIN_ID --node $AKASH_NODE --owner $AKASH_ACCOUNT_ADDRESS --dseq $AKASH_DSEQ --provider $AKASH_PROVIDER --from $AKASH_KEY_NAME --fees 5000uakt

# Create a deployment 
akash tx deployment create substrate.yaml --from akash145kmcq2zuqlrzj6raa9p86ukjclsp7prr59x0y --node $AKASH_NODE --chain-id $AKASH_CHAIN_ID --fees 5000uakt -y

# Get bid list
akash query market bid list --owner=akash145kmcq2zuqlrzj6raa9p86ukjclsp7prr59x0y --node $AKASH_NODE --dseq $AKASH_DSEQ

akash query authz grants akash145kmcq2zuqlrzj6raa9p86ukjclsp7prr59x0y akash1jq42qysz9tnwa7my645qt2eg4gm8fgn39pmxtr


akash tx authz grant akash145kmcq2zuqlrzj6raa9p86ukjclsp7prr59x0y send --spend-limit=50akt --from akash1jq42qysz9tnwa7my645qt2eg4gm8fgn39pmxtr --fees 5000uakt

akash tx deployment create substrate.yaml --from akash145kmcq2zuqlrzj6raa9p86ukjclsp7prr59x0y --node $AKASH_NODE --chain-id $AKASH_CHAIN_ID --fees 5000uakt -y --fee-account akash1jq42qysz9tnwa7my645qt2eg4gm8fgn39pmxtr
