# GitLab

GitLab specific documentation.

## Repository settings

### SSH Key Pair

To ensure our pipelines has read/write access to our GitLab repository, we need to create an public key pair and add this to our project. This Key Pair could also be used to connect to remote servers if neccesery.

To create a Key Pair we will be using `ssh-keygen`. You can create a keypair using the following command `~ $ ssh-keygen -f GitLabCi`. Make sure to specify a new file name so you don't overwrite your main key-pair! The easiest way is to create a ssh-key without a password.

- Upload the key under: `Project Settings -> Repository -> Deploy Keys` make sure to tick the checbox for write access if needed.
- Create an environment variable for the private key under: `Project Settings -> CI / CD -> Variables`
