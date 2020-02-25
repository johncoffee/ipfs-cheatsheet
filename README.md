# ipfs-cheatsheet

A handy collection of snippets. Official reference here https://ipfs.io/docs/commands/


# Repo management

## Remove all pins 

`ipfs pin ls -q --type recursive | xargs ipfs pin rm`

`ipfs pin ls --type recursive | cut -d' ' -f1 | xargs -n1 ipfs pin rm`

# Deployment / tools

`npx ipfs-deploy` (defaults to Infura, but they have some size limit so maybe it'll just pin a random file!)

`npx ipfs-deploy -p pinata ./public` (needs .env with pinata keys)

