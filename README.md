# GitProfileManager
**Git extension to provide a profile manager.**

GitPM permits to easily select a git profile before commit.
Useful if you have multiple git repositories with multiple identities.

Thanks to [lodi-g](https://github.com/lodi-g) :heart: - Main Contributor

## Installing

To install:

```
bash < <(curl -s -S -L https://github.com/si0ls/GitProfileManager/raw/master/installer)
```

To uninstall:

```
sh ~/.gitpm/installer uninstall
```

## How does GitPM works

### Usage

#### Get usage:

```
git pm -h
```

#### Add a profile:

```
git pm add [-h] -p PROFILE -n NAME -m MAIL
```

#### Remove a profile

```
git pm rm [-h] -p PROFILE
```

#### List existing profiles

```
git pm list [-h]
```

#### Select current git repository profile

```
git pm select [-h] -p PROFILE
```

#### Commit with a profile (restore the old profile after comitting)

```
git pm commit [-h] -p PROFILE ...
```

### Git Hook

GitPM comes with a git hook on commit, asking wich profile to use for the current git repository if not defined.
