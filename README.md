# WARNING

Never, ever just clone this repo and trust the pubkeys! Use the last-known good SHA instead. See the *How to use* section below.

## The problem

The Identity team builds test/dev tools using one-off AWS instances. Some of these tools become indispensable, yet, don't warrant being monitored and managed by ops.

In the past, tools have broken down while their creators were on vacation or unavailable, leading to bummer-times for everybody involved--either sshing into a box while on PTO, or the tool just being borked for days.

## The solution

This repo contains public keys for the Identity core crew.

If toolmakers upload their fellow devs' pubkeys to a long-lived awsbox, anybody can reboot or troubleshoot a downed machine when its creator is out on vacation.

*Yay vacation.*

## How to use 

Only use the pubkeys from the latest SHA which has been verified as good by the core Identity team. (This happens in email, not in github.)

## When to use

If you create a tool on an awsbox that someone might need to maintain while you're away, then you can upload the identity-pubkeys to that awsbox and relax.

## How to update with new keys

If people join the team and you add keys to this repo, you must notify the team via the mailing list and ask everyone to verify their keys are correct in the version identified by the new HEAD SHA.

We trust github and git because you can't modify the keys without also changing the SHA.
