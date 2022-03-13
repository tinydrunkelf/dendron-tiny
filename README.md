# TinyDrunkElf's Dendron site for notes

[SITE HERE](https://tinydrunkelf.github.io/dendron-tiny/)

## Dendron
- https://github.com/dendronhq/dendron-site - site example
- https://www.dendron.so/ - dendron home

## Git setup

### git config setup
```bash
# ./.git/config
[include]
	path = ../.gitconfig
```
- <https://stackoverflow.com/questions/18329621/how-to-store-a-git-config-as-part-of-the-repository#18330114>

### local git configuration
```bash
# ./.gitconfig
# note: this is NOT in ./.git/config (that file is above)
[user]
	email = 100638235+tinydrunkelf@users.noreply.github.com
	name = tinydrunkelf
[core]
...
	editor = vim
	sshCommand = "ssh -i ~/.ssh/id_gh_tinydrunkelf"
...
```
- Declare the remote config
- Use a no-reply email from github
    - <https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-github-user-account/managing-email-preferences/setting-your-commit-email-address>
- Set a reference to the private ssh key, register public key with GitHub
     - <https://dev.to/web3coach/how-to-configure-a-local-git-repository-to-use-a-specific-ssh-key-4aml>
    - <https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent#adding-your-ssh-key-to-the-ssh-agent>

### More info on `git` `[includes]`
- <https://blog.thomasheartman.com/posts/modularizing-your-git-config-with-conditional-includes/>
- <https://git-scm.com/docs/git-config#_conditional_includes>