# coop

We share our passwords via an encrypted repo on Keybase. This is our CLI to
access them.

## Usage

Simply call `coop` with the name of the service you wish to copy.

```shell
coop netflify
```

## File format

Our password files need to have a specific format. Example, for `netlify`:

```
username: our-username
password: our-password
```

## Install

```shell
wget https://raw.githubusercontent.com/cooperativa-tech/coop/master/coop
mv coop /usr/local/bin/ # or another directory that is in your `$PATH`
```

The tool allows the definition of a `$COOPERATIVA` environment variable that
points to a directory with the `secrets` project. This allows you to cache the
project without having the tool clone it repeatedly.

```shell
# For zsh:
echo "export COOPERATIVA=$HOME/Developer/cooperativa" >> ~/.zshrc

# for bash
echo "export COOPERATIVA=$HOME/Developer/cooperativa" >> ~/.bashrc
```
