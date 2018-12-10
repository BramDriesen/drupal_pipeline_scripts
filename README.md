# Drupal Pipeline Scripts

The goal of this repository is to create a collection with examples of how to build and deploy your Drupal 8 project starting from your `composer.json` file. This means there is no need to add any of the contributed modules or vendor libraries into your `git` repository.

The build process will thus collect all required dependencies, apply patches and deploy the code to your repository.

NOTE: This is still a WIP :) feel free to help out!

## Outline

TODO

## General information

The examples provided by this repository are (currently) only the fundementals to build the source code for a Drupal 8 site with composer. In a real life situation you *should* add more functionality to the build/test steps. A few examples of things that you can implement:
- Running [PHP Code Sniffer][2] and [PHP Mess Detecor][3] (and reject the build if there are issues)-
- Running Complexity checks like: [PhpMetrics][1]
- Running automated tests like: [Behat][4], [PHPUnit][5]
- Compiling your SASS/LESS files
- ...

It's also possible to execute tasks on the destination server after the code has been deployed to automate your process even further. Some things you could do:
- Execute database updates
- Import configuration
- Clear caches
- ...

The items mentioned above are just a few of the many cool thigns you could do to automate your workflow.

## Covered repositories

- Bitbucket
- GitLab

## Basic build steps

- Composer install
- Transfer code to destination


## Ways of transfering

The ways of transfering code from your build to your destination server depends on the capabilities of the destination. For example, cheap hosting providers often don't offer GIT or SSH Access and only allow file transfers to be made ofer `FTP/SFTP`. 

While other, often more expenive hosting providers allow you to use their Git repository, but most of the times don't offer an Git UI, which will make teamwork and code reviews a nightmare. So what you want to do is create your main repositorty somewhere else (E.g BitBucket or GitLab) and "mirror" the code to the cloud servers.

If you happen to be using services like AWS/Google Cloud/Azure to host your website, you'll probably also have the option to just transfer the files over SSH/SCP.

Some of the possibilities are:

- Git
- SSH/SCP
- FTP

### Git

git commit -> push ?
git tag -> push ?

### SSH/SCP

Rsync?
SCP?

### FTP

Git FTP? 
csync ? 
lftp ? < 
ncftp ? 


## Disclaimer

I'm in no way affiliated with any of the mentioned hosting providers, Git Reposities or any other names mentioned. I'm just trying to cover some of the more popular solutions which are commonly used these days.


[1]: https://www.phpmetrics.org
[2]: https://github.com/squizlabs/PHP_CodeSniffer
[3]: https://phpmd.org
[4]: http://behat.org/en/latest
[5]: https://phpunit.de
