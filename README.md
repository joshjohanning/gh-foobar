# gh-foobar

This is an example of a bash `gh cli` extension. You can also use this example to call a PowerShell script, if that's your preferred language, with the `pwsh` command. 

<img width="520" alt="gh-foobar" src="https://user-images.githubusercontent.com/19912012/194949817-b0b97b95-a2cf-4f49-b89a-9db8d591e24b.png">

## How this was created

1. Create template: `gh extension create --precompiled=other foobar`
2. cd into the `gh-foobar` dir, clean up files, add shell script/etc.
    - Shell script in root must start with: `#!/usr/bin/env bash` 
3. Install 
    - Install local copy of extension with: `gh extension install .`
    - Install remote version of extension with: `gh extension install joshjohanning/gh-foobar`
4. Execute with `gh foobar`
5. If needed, to remove: `gh extension remove gh-foobar`
6. Note: Local extensions cannot be upgraded, you have to remove and re-install, but otherwise upgrade extension with `gh extension upgrade joshjohanning/gh-foobar`

See [here](https://cli.github.com/manual/gh_extension) for a list of all `gh extension` options. 
