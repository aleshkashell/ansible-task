Storage
=========

Role provides possibility to encrypt drive and partition. Role checks if you try to encrypt root partition and it will fail in this case.

Requirements
------------

`jq` tool is required for detection of the drive which contains root partition. It will be installed in context of this role

Role Variables
--------------

- `enc_drive_name` - name of the drive to encrypt
- `enc_partition_name` - name of the partition to encrypt
- `crypt_passphrase` - secret for encryption

Dependencies
------------

It depends on `community.crypto` collection

