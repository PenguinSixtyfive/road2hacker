# Connecting using keys

After copying the pub key to the server, you can connect to the server using the private key:

```bash
ssh -i .ssh/<key> <user>@<server>
```

An easier way to connect to a server is:
1. Make a config file in `$HOME/.ssh/`, then in it type:
> Host <shortcut name>
    > User <username>
    > HostName <server
    > IdentityFile $HOME/<path to priv key>

To connect:
```bash
ssh <shortcut name>
```
