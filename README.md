# Drupal Pipeline Scripts

The goal of this repository is to create a collection with examples of how to build and deploy your Drupal 8 project starting from your `composer.json` file. This means there is no need to add any of the contributed modules or vendor libraries into your `git` repository.

The build process will thus collect all required dependencies, apply patches and deploy the code to your repository.

NOTE: This is still a WIP :) feel free to help out!

## Covered repositories

- Bitbucket
- GitLab

## Basic build steps

- Composer install
- Transfer code to destination


## Ways of transfering

The ways of transfering code from your build to your destination server depends on the capabilities of the destination.

Some of the possibilities are:

- Git
- SSH
- FTP

### Git

git commit -> push ?
git tag -> push ?

### SSH

Rsync?

### FTP

Git FTP? 
csync ? 
lftp ? < 
ncftp ? 
