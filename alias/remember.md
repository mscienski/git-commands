```[alias]
	aliases = !git config --get-regexp 'alias.*' | colrm 1 6 | sed 's/[ ]/ = /' | sort```
