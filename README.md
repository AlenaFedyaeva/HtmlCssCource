# HtmlCssCource
In each folder you can find task.txt file with homework task

How to install brackets on debian(libcurl3 libcurl4 problem solved)
1) Download the .deb installer file
2) Inside the folder your downloaded the file run dpkg-deb -R ./Brackets.Release.1.12.64-bit.deb Brackets
3) Edit file Brackets/DEBIAN/control and replace libcurl3 with libcurl4
4) Rebuild .deb installer running dpkg-deb -b Brackets Brackets-fixed.deb
5) Install Brackets using the fixed installer running sudo dpkg -i Brackets-fixed.deb
