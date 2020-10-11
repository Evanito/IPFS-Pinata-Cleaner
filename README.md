# IPFS-Pinata-Cleaner
Python script to clean up duplicate folders uploaded to https://pinata.cloud

## Introduction
Tools such as IPFS Deploy leave a lot of previous hashes uploaded to Pinata.\
This script simply checks your hashes, and only keeps the most recent of files that share the same name.

Add this to your IPFS Deploy deployment pipeline to automate cleanup!

## Usage
From your CLI:\
`python pinata_cleanup.py -a <pinata_api_key> -s <pinata_api_secret> -c <how_many_to_keep_of_same_name>`

And that's really it!

## Future plans

- Cache to disk old pins for users with a large amount of pins?
- Allow to filter based on a Pinata tag?
- Allow to filter based on a Pinata tag's value?