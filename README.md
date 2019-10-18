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

```
wget file
mv file /usr/local/bin/ # or another directory that is in your `$PATH`
```
