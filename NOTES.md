### 1. Create key
solana-keygen new --outfile ~/.config/solana/devnet.json

### 2. Set default key
solana config set --keypair ~/.config/solana/devnet.json

### To change collection delete .cache folder

### Upload to metaplex
ts-node ../metaplex/js/packages/cli/src/candy-machine-v2-cli.ts upload -e devnet -k ~/.config/solana/devnet.json -cp config.json ./assets

### Update metaplex (candy machine)
ts-node ../metaplex/js/packages/cli/src/candy-machine-v2-cli.ts update_candy_machine -e devnet -k ~/.config/solana/devnet.json -cp config.json

### Verify 
cmd = verify

### areweave solana storage fee calc
https://arweavefees.com/
