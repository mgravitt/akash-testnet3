# Environment vars

AKASH_VERSION=v0.15.0-rc14

AKASH_NET="https://raw.githubusercontent.com/ovrclk/net/master/edgenet"
export AKASH_KEYRING_BACKEND=os
export AKASH_NODE="$(curl -s "$AKASH_NET/rpc-nodes.txt" | shuf -n 1)"
export AKASH_CHAIN_ID="$(curl -s "$AKASH_NET/chain-id.txt")"

AKASH_KEY_NAME=testnet3

akash keys add $AKASH_KEY_NAME

export AKASH_ACCOUNT_ADDRESS="$(akash keys show $AKASH_KEY_NAME -a)"

echo $AKASH_ACCOUNT_ADDRESS

# First Account
- name: testnet3
  type: local
  address: akash145kmcq2zuqlrzj6raa9p86ukjclsp7prr59x0y
  pubkey: '{"@type":"/cosmos.crypto.secp256k1.PubKey","key":"AgPXjPYDrmIfVOPEEq53ljTJTQsFvC3fDP2/8XtKBsJY"}'
  mnemonic: ""

rifle now brave soft original fatigue dizzy glass timber jacket bachelor ride mercy space panic forward biology carry capital sword giggle salad claim increase

# Second Account
- name: testnet3-1
  type: local
  address: akash1jq42qysz9tnwa7my645qt2eg4gm8fgn39pmxtr
  pubkey: '{"@type":"/cosmos.crypto.secp256k1.PubKey","key":"Aj/kqDg9WFAVJnDyNf0qrfgUpHX26r2Nn7pRTWH3doE8"}'
  mnemonic: ""

slice undo farm guilt chalk amazing hair keep small brain health cart develop diet repair current ivory open regret destroy nice artist wet snake


AKASH_KEYRING_BACKEND=os

export AKASH_ACCOUNT_ADDRESS="$(akash keys show $AKASH_KEY_NAME -a)"

{"transactionHash":"B30B5D33E3D0EA1CAC40F4BFAA5C1E4B2B4A6F543540288D05E2AEC03C32466B"}