# Setup System



### ssh without pwd
On the desktop ```ssh-keygen```

Copy key to the server ```ssh-copy-id not-marco@server```

##### avoid ssh asking permission
Set ```StrictHostKeyChecking``` no in your /etc/ssh/ssh_config file


##### assign server name instead of ip
```sudo vim /etc/hosts```, add line ```128.90.111.135 myubuntu```


##### latex
```sudo apt-get install texlive-full```

```sudo apt-get install texlive-fonts-recommended```

```sudo apt-get install texlive-fonts-extra```

##### resize images
```sudo apt-get install imagemagick```

```mogrify -resize 50% *.png   # keep image aspect ratio```

```mogrify -resize 320x240! *.png``` Don't keep aspect ratio.


### Leaving Blank

Shu Kong @ UCI
Sep. 2018

