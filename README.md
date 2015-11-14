# bash

Hello guys! 

This repository contains two script codes written in bash that can be used in our daily work. Should anyone happen to like or trust command line more than online tools or just to double-triple-check, this will help you to avoid typing different requests in PuTTY making alltogether in two clicks.

I uploaded the codes in txt format so that the content can be copied and pasted into your roaming profile.

The first code named <code>all.txt</code> includes all common commands SSL CS specialists are using to check a domain. In the output you will see DNS records, redirection rules if any, availability of ports and ciphers used by the server (special thanks to Anton Ku. for his article about nmap), SSL handshake process and openssl checks with SNI argument.

The second one <code>host.txt</code> simply performs reversed IP resolution and identifies a name of server which hosts a requested domain.

In order to make them work on your machine, please run <code>nano filename.sh</code> command in the terminal. <code>.sh</code> is a mandatory extension. You can select any name for your file replacing "filename". This command will start a text editor. Copy the code from txt file and paste it into the terminal. Once it is done, click Ctrl+O that saves changes, confirm the filename typing "Y" or change it and Ctrl+X that exits Nano editor.

After that the file must be marked as executable. This can be done with quick chmod. Type <code>chmod u+x filename.sh</code> in PuTTY. The script can be run now with ./ syntax, for instance <code>./all.sh</code>.

You can also configure an alias for it, if you wish to run the code with one word. Open the configuration file of your PuTTY with <code>nano .bash_profile</code> command. Type, for example <code>alias all="./all.sh"</code>. Exit with Ctrl+O and Ctrl+X. This will create a permanent alias for <code>./all.sh</code> command. Then type <code>source ~/.bash_profile</code> command. It will reload the shell and allow running newly created alias without restarting terminal a session.

That's it! Feel free to use and modify it soever.
