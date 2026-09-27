# import_maildir_mox
Recursively import an existing maildir into mox mail server.

> [!WARNING]
> Not responsible for data loss. Always have backups and verify what is proposed
> before executing command. Though thoroughly tested and used, there still may be
> bugs that cause data loss.

Maildir must be in a Mox accessible location with correct permissions.
Typically this is /var/opt/mox/data. Execute from the Mox root directory.

## Import example
``` bash
# Run without paramters for help.
./import_maildir_mox

./import_maildir_mox -f -p example_user Archive/migration data/import/Maildir/
Source Maildir:     /var/opt/mox/data/import/Maildir
Target Account:     example_user
Target Import Root: Archive/migration
Press enter to continue (ctrl+c to exit)
----------------------------------------
Maildir:  /var/opt/mox/data/import/Maildir/.All Mail
Target:   Archive/migration/All Mail
Messages: 29349 (~908M)
[SUCCESS]: 29349 messages successfully imported.
----------------------------------------
Maildir:  /var/opt/mox/data/import/Maildir/.Drafts
Target:   Archive/migration/Drafts
Messages: 3 (~44K)
[SUCCESS]: 3 messages successfully imported.
----------------------------------------
Maildir:  /var/opt/mox/data/import/Maildir/.Important
Target:   Archive/migration/Important
Messages: 4230 (~282M)
[SUCCESS]: 4230 messages successfully imported.
----------------------------------------
Maildir:  /var/opt/mox/data/import/Maildir/.Sent Mail
Target:   Archive/migration/Sent Mail
Messages: 717 (~242M)
[SUCCESS]: 717 messages successfully imported.
----------------------------------------
Maildir:  /var/opt/mox/data/import/Maildir/.Spam
Target:   Archive/migration/Spam
Messages: 1 (~56K)
[SUCCESS]: 1 messages successfully imported.
----------------------------------------
Maildir:  /var/opt/mox/data/import/Maildir/.Starred
Target:   Archive/migration/Starred
Messages: 64 (~3.9M)
[SUCCESS]: 64 messages successfully imported.
----------------------------------------
Maildir:  /var/opt/mox/data/import/Maildir/.Trash
Target:   Archive/migration/Trash
Messages: 2056 (~182M)
[SUCCESS]: 2056 messages successfully imported.
----------------------------------------
Maildir:  /var/opt/mox/data/import/Maildir/.old.archive
Target:   Archive/old/archive
Messages: 231841 (~15G)
[SUCCESS]: 231841 messages successfully imported.

...

Import complete.
```

## Issues
Create a bug and provide as much information as possible.

Associate pull requests with a submitted bug.

## License
[AGPL-3.0 License][c] | [direct link][f]

## Author Information
PGP: [466EEC2B67516C7117C85CE3A0BC35D16698BAB9][d] | [github gist][e]

[c]: https://www.tldrlegal.com/license/gnu-affero-general-public-license-v3-agpl-3-0
[d]: https://keys.openpgp.org/vks/v1/by-fingerprint/466EEC2B67516C7117C85CE3A0BC35D16698BAB9
[e]: https://gist.github.com/r-pufky/a8df36977c55b5bb20829267c4c49d22
[f]: https://github.com/r-pufky/ansible_paperless_ngx/blob/main/LICENSE
