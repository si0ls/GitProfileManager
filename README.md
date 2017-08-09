# GitProfileManager
**Git extension to provide a profile manager.**

GitPM permits to easily select a git profile before commit.
Useful if you have multiple git repositories with multiple identities.

Thanks to [lodi-g](https://github.com/lodi-g) :heart: - Main Contributor

## Installing

To install:

```Bash
bash < <(curl -s -S -L https://github.com/si0ls/GitProfileManager/raw/master/installer)
```

Or if you are using zsh:

```Bash
zsh < <(curl -s -S -L https://github.com/si0ls/GitProfileManager/raw/master/installer)
```

To uninstall:

```Bash
sh ~/.gitpm/installer uninstall
```

## How does GitPM works

### Usage

#### Get usage:

```Bash
git pm -h
```

#### Add a profile:

```Bash
git pm add [-p profile_name -n name -m mail]
```

*If parameters are missing, will be interactive in V2.0*

#### Remove a profile

```Bash
git pm rm [profile_name]
```

*If parameters are missing, will be interactive in V2.0*

#### List existing profiles

```Bash
git pm list
```

#### Select current git repository profile

```Bash
git pm select [profile_name]
```

#### Comming Soon V2.0 : Commit with a specific profile (one time)

```Bash
git pm commit [--profile profile] [git options]
```

*If parameters are missing, will be interactive in V2.0*

### Git Hook

GitPM commes with a git hook on commit, asking wich profile to use for the current git repository if not defined.