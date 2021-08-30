# AbracaCIDRa - Sensible cloud network layouts for people who don't care about network layout

## What Is This For?

AbracaCIDRa takes a definition of network hierchy parameters, (example: Region,
availability zone, an purpose), and produces a network layout in the form of
JSON that can be referenced instead of that awful network spreadsheet or giant
IPAM.

## What Is This For? (The Long Version)
Has this ever happened to you?  You are creating a new subnet in a VPC and you
have no idea what space is free, and you worry about the subnet size being
too small or too large, and you lost that spreadsheet someone made 3 years ago
called "network master plan - v0.1", so you end up wasting an hour digging
around to find space.

Wouldn't it be nice to be able to provide a few parameters describing the
new subnet and get back a private IPv4 CIDR block?  Wouldn't it be better
if you could do the same for multiple regions, or cloud providers, and have
some assurance you were not laying a trap for your future self that you need
to NAT or route table hack your way round?

## TODO

* Basic network layout generator
* Sample network
* No-go-zones - Allow defining networks that can not be in the automatic layout
* CLI for forward and reverse lookups
* Sample use with Terraform and no IPs in code


