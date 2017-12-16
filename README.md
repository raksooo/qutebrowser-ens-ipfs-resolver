# ENS to IPFS resolver Qutebrowser userscript
This Qutebrowser userscript makes it possible to browse .eth domain which are registered in Ethereum name service (ENS) and has a IPFS object connected to it.
Learn more about ENS and register your domain [here](https://ens.domains/).
Set IPFS content hash for your ENS domain [here](https://monkybrain.github.io/ipfs-to-ens/)

## Dependencies
* [ens-ipfs-resolver](https://www.npmjs.com/package/ens-ipfs-resolver)

## Installation
```
git clone https://github.com/raksooo/qutebrowser-ens-ipfs-resolver.git
ln -s $(pwd)/qutebrowser-ens-ipfs-resolver/qutebrowser-ens-ipfs-resolver ~/.local/share/qutebrowser/userscripts/ens-ipfs-resolver
```

## Usage
Unfortunately Qutebrowser does not support automatically running userscripts. When you browse to a .eth domain you will end up on a 404-page. From there you run the command
```
spawn --userscript ens-ipfs-resolver
```

To make it a bit less tedious it is possible to create a keybinding in your config.py:
```
config.bind('e', 'spawn --userscript ens-ipfs-resolver')
```

