# ipfs-cheatsheet

A handy collection code. Official reference here https://ipfs.io/docs/commands/

# Repo management

## Remove all pins 

`ipfs pin ls --type recursive | cut -d' ' -f1 | xargs -n1 ipfs pin rm`
