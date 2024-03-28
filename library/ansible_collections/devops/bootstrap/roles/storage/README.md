Storage
=========

Role provides possibility to encrypt drive and partition. Role checks if you try to encrypt root partition and it will fail in this case.

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------

`enc_drive_name` - name of the drive to encrypt
`enc_partition_name` - name of the partition to encrypt
`crypt_passphrase` - secret for encryption

Dependencies
------------

It depends on `community.crypto` collection

