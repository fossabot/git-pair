# git-pair [![Build Status](https://travis-ci.org/augustohp/git-pair.svg)](https://travis-ci.org/augustohp/git-pair)
[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2Faugustohp%2Fgit-pair.svg?type=shield)](https://app.fossa.io/projects/git%2Bgithub.com%2Faugustohp%2Fgit-pair?ref=badge_shield)

Simple bash-script allowing pair to be identified on git commits:

    $ git pair "Nelson Senna"

From now on, your commits will be identified with authors like:

    commit a101286e02117fdafea58742074694138d578948
    Author: Augusto Pascutti + Nelson Senna <augusto@phpsp.org.br>
    Date:   Thu Sep 3 23:00:58 2015 -0300

You can use as many pairs you want, all you need is keep issuing
commands to add more authors.

    git pair ended

At the end of your pairing session, the above command will reset
author names to your global `user.name` configuration on Git.

## Installation

One-liner using [Sinister](https://github.com/jamesqo/sinister):

    $ sh <(curl -sSL http://git.io/sinister) --local --url https://git.io/git-pair

Or you can clone the project where you want to, all you need after
is to sym-link the `git-pair` script to your `$PATH`:

    $ cd <my-src-dir>
    $ git clone http://github.com/augustohp/git-pair
    $ chmod a+x git-pair/git-pair
    $ ln -s <my-src-dir>/git-pair /usr/local/bin

Now you should be able to execute `git pair` anywhere.


## License
[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2Faugustohp%2Fgit-pair.svg?type=large)](https://app.fossa.io/projects/git%2Bgithub.com%2Faugustohp%2Fgit-pair?ref=badge_large)