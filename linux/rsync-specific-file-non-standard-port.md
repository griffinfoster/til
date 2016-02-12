# rsync specific filetypes using non-standard SSH port

To rsync python pickle files using port 2223:

`rsync -azv --stats -e "ssh -p 2223" --include "*.pkl" --include '*/' --exclude "*" --prune-empty-dirs username@host:/path/to/files/ /local/path/to/files/`
