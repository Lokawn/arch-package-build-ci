# Add following secrets to the repo:
    - SSHKEY : Private ssh key with newlines replaced by newline character (\n). Add public key remote server.
    - PRIVATE_KEY : GnuPG private key with newlines replaced by newline character (\n).
    - PUBLIC_KEY :  GnuPG public key with newlines replaced by newline character (\n).
    - KEY_FINGERPRINT : GnuPG private key fingerprint.
    - PASSPHRASE : Passphrase associated with GnuPG secret key.
    - REMOTE : Location of remote repository. Rsync syncs contents of folder if a trailing slash is present in remote name, otherwise a new folder with basename of remote is created inside destination directory.
    - HOST : Public SSH key of remote host, which is appended to .ssh/known_hosts.

## SSH private key is put in .ssh folder as default SSH key.
## GnuPG private key is used to sign package files.
## GnuPG public key is used to verify package file signatures.
## Fingerprint is used to verify GnuPG secret key is present in database.

- ENABLE_DEBUG : Set this repository variable true to enable debug logs.