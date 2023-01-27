kver
=======

Switch between kubectl versions by specifying version or   
automatically based on context.   
Currently for mac only.   
   
Meant to replace your `alias k='kubectl'`.   
If you have this alias set, you'll need to comment out or remove.   
   
kver will set the 'k' command to be soft-linked to the kubectl version to be used.   
They are stored in your ~/.kver directory.   

kver Installation:
```
unalias k
mkdir ~/.kver
echo 'export PATH="~/.kver:$PATH"' >> ~/.bashrc
source ~/.bashrc
curl https://raw.githubusercontent.com/tkjef/kver/master/kver -o ~/.kver/kver
chmod +x ~/.kver/kver
```

Usage:
```
$ kver <version>

EXAMPLES:
    kver 1.22.9
    kver - # switch to previous version
```

## Author

Created &amp; maintained by [tkjef][tkjef] (<yo@tkjef.com>).  

## License

MIT License, (see [LICENSE][license])

[contributors]: https://github.com/tkjef/kver/graphs/contributors
[tkjef]: https://github.com/tkjef
[issues]: https://github.com/tkjef/kver/issues
[license]: https://github.com/tkjef/kver/blob/master/LICENSE
[twitter]: https://twitter.com/tkjef
[website]: http://www.tkjef.com/

## Project Roadmap

Version 0.2.0  
    -add optional - flag for switching to previous kubectl version   
    -more error checking   
    
Version 0.3.0   
    -setup brew install    
