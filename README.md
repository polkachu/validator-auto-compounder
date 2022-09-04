# Validator Auto Compounder for Tendermint-Based Chains

> In the validator world, rich gets richer. -Polkachu

## Why

As a degen validator, you sometimes want to auto-compound the rewards right after the genesis time to gain tiny advantages over other validators. Being slightly above other validators on the ranking chart will have implications on your long-term ranking.

## How

First, make your own inventory file by copying the sample inventory file.

```bash
cp inventory.sample inventory
```

Then, update some variables to your liking.

Finally, run

```bash
ansible-playbook main.yml
```

NOTE: This playbook is designed to be one-off and the inventory file is meant to be ephemeral. When you have a secondary node to auto-compound, you just change the inventory file for the second node.
