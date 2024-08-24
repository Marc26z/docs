# FAQ

## General Questions

### What is Lightning.Pub?

"Pub" is a Nostr-native account system designed to make running Lightning infrastructure for your friends/family/customers easier than previously thought possible.

Pub also features a management dashboard for node runners, and allows the sending of guest invitations to your node. This makes ShockWallet the best Lightning wallet for users of all levels, from the node runner looking to share access with family, to the passive guest user that just wants a fast and reliable custodial experience and trust their friends over a big company.

## Can I import an backup?

You can backup and restore the db.sqlite file in the lightning_pub directory and introspect it to recover seed and encryption phrases, but we do not yet have automatic tooling for recoveries at this time. Contact us for support.

Lightning recoveries in general are disaster recovery scenarios given the nature of channel states, we recommend a highly available system with a battery to facilitate graceful disk shutdowns. 

## Transactions

### How do I send on-chain Bitcoin?

On-chain spends are not yet supported while the software matures, you should use lncli on the underlying LND instance for the time being.

## Lightning Network

### How do I open a Lightning channel?

This feature is coming soon to the integrated Lightning.Pub Dashboard, to access the dashboard, tap the logo in ShockWallet 3 times if you are connected as the node administrator.

Alternatively, you may use lncli from the command line to manipulate the underlying LND instance.

### Does it use ECash? How does it compare on privacy?

No, in our view ECash makes deceptive privacy claims while combining the worst trade-offs in combining a custodial solution with bearer credentials. 

Lightning.Pub eschews flakey mint gateways fpr a much more reliable, and equally private, direct RPC approach. Nostr keys used for connections are source ephemeral and blind to social parent keys that may be used to perform backups. Settlement to and from ECash mints works as long as those mints are actually backed by Lightning.

Privacy equivalence aside, we do not an endorse **any** custodial Lightning services for privacy. A node operator has countless ways to deanonymize activity, and you should not use a node if you do not trust the operator with your metadata. 

## Security

### How safe is Lightning.Pub?

Any wallet connected to the internet is a **"hot wallet" and should not be used to store life changing amounts of Bitcoin.** We believe Lightning.Pub to be as, if not more, secure than any other Lightning account system available, but this is a bleeding edge software in a bleeding edge ecosystem and there will be vulnerabilities.

## Troubleshooting


## Support

### Where can I get help with ShockWallet?

See below for our online forums, or for more private options see our [contacts](https://docs.shock.network/contact). 

### How do I report a bug?

- For security vulnerabilities, please use the [security advisor feature](https://github.com/shocknet/Lightning.Pub/security/advisories) on the Github repository.
- For all other issues, please use [Github issues](https://github.com/shocknet/Lightning.Pub/issues).

### Is there a community forum for ShockWallet users?

Yes, you can join the Lightning.Pub community through:
- Telegram: [t.me/ShockBTC](https://t.me/ShockBTC)
- Github Discussions: [https://github.com/shocknet/Lightning.Pub/discussions](https://github.com/shocknet/Lightning.Pub/discussions)