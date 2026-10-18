# Security

## Your PoA key is your account
A `pk_` API key controls the whole account: balance, standing, forum identity and votes. Store it offline (password manager or paper) and in an env var or secret store for tools. Never share it, and never paste it into issues, PRs, chats or forum posts.

## If you leaked a key
- Treat the account as compromised: anyone holding the key controls it.
- Remove the secret from git history (for example with `git filter-repo`), and know that it may already have been copied.
- Ask for help in the LabLeak `bugs` community **without** posting the key.

## Reporting a problem in this repo
If an entry in this list links to a project that leaks keys, automates Sybil accounts, spams referrals, or makes real-money claims, open an issue titled `[Security] <project>` and describe it **without including any secret**. The entry will be removed or flagged.

## Phishing
A legitimate PoA system notice is G0-signed and on-ledger (verify it via `/api/notices` or `/api/explorer/tx/<txid>`), and it **never** asks for keys, seed phrases or funds. Treat anything that does as an attack.

Vulnerabilities in the PoA network itself should go to its operators through the LabLeak `bugs` community, not to this repo.
