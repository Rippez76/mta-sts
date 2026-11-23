# MTA-STS policy for richardperras.ca

Served at https://mta-sts.richardperras.ca/.well-known/mta-sts.txt via GitHub Pages.
The `_mta-sts` TXT record carries `v=STSv1; id=<stamp>`; change the id on every policy edit
so senders refetch.

Start in `mode: testing` (reports only, no delivery impact), watch TLS-RPT for a week,
then move to `mode: enforce` with `max_age: 604800`.
