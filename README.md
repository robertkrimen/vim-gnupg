This is a fix to gnupg.vim that allows the use of gpg-agent with pinentry-curses

If this fits your use case, then set ```g:GPGPrimeAgent``` to 1 in your ```.vimrc``` to
enable priming of gpg-agent:

    let g:GPGPrimeAgent = 1

http://gitorious.org/vim-gnupg/vim-gnupg

# vim-gnupg

This script implements transparent editing of gpg encrypted files. The
filename must have a ".gpg", ".pgp" or ".asc" suffix. When opening such
a file the content is decrypted, when opening a new file the script will
ask for the recipients of the encrypted file. The file content will be
encrypted to all recipients before it is written. The script turns off
viminfo and swapfile to increase security.
