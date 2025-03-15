# HOMELAB

## SSH configuration

Configure SSH key authentication to the server by generating an SSH key pair locally and copy the public key over to the remote host.
~~~bash
$ ssh-keygen -t ed25519 -f '$HOME/.ssh/homelab' -N '' -C 'robert-homelab'
$ ssh-copy-id -i '$HOME/.ssh/homelab' robert@IP_ADDR
~~~
