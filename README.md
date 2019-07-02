# My GPG Keys

This page contains information about my GPG keys.

## Checking Keys and Download

You can check my up-to-date keys at https://api.github.com/users/vancluever/gpg_keys.

To fetch just the key you can use `curl` and `jq`:

```
curl -s https://api.github.com/users/vancluever/gpg_keys | jq -r .[0].raw_key
```

## Current Keys

```
$ curl -s https://api.github.com/users/vancluever/gpg_keys | jq -r .[0].raw_key  | gpg -v 2>/dev/null
pub   rsa4096/21DA69C2D14BFAA8 2017-07-24 [SC] [expires: 2024-06-24]
      Key fingerprint = 245C DB0E 5171 60F3 EBC5  6923 21DA 69C2 D14B FAA8
uid                           Chris Marchesi <chrism@vancluevertech.com>
sig        21DA69C2D14BFAA8 2019-06-26   [selfsig]
sub   rsa4096/8D6F1589D9834498 2017-10-16 [S] [expires: 2024-06-24]
sig        21DA69C2D14BFAA8 2019-06-26   [keybind]
sub   rsa4096/34A2AF5F60B91FA1 2017-07-24 [E] [expires: 2024-06-24]
sig        21DA69C2D14BFAA8 2019-06-26   [keybind]
sub   rsa4096/335B84AFEC615CE4 2017-07-25 [S] [expires: 2024-06-24]
sig        21DA69C2D14BFAA8 2019-06-26   [keybind]
```
