# subversion-hooks

Allows [subversion](https://subversion.apache.org/) to call multiple hooks!

## Setup

You need to configure your SVN repository with the hook.

Note the following requirements:
- `/path/to/svn-repo/` *MUST* end in a slash (`/`) to ensure that it is a directory

1. Clone
1. Run `make debian-package-dependencies` to install dependent *build* Debian packages
1. Run `make debian-package` to build package locally
1. Run `dpkg -i package/subversion-hooks_X.X.X_all.deb` to install package locally
- [SVN](https://subversion.apache.org/)
1. add the hook to the repository
    ```
    add-subversion-hooks /path/to/svn-repo/
    ```

## License

Copyright 2024 by carrvo

License: [Unlicense](https://choosealicense.com/licenses/unlicense/) (also known as public domain).

