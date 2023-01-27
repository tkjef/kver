kver
=======

Switch between kubectl versions quickly and automatically based on context. Currently for mac only.  

kver Installation:
```
mkdir ~/.kver
echo 'export PATH="~/.kver:$PATH"' >> ~/.bashrc
curl https://raw.githubusercontent.com/tkjef/kver/master/kver -o ~/.kver/kver
chmod +x ~/.kver/kver
```

Usage:
```
$ kver <version> [-x <kubectx context> ] [-n <kubens namespace]   

REQUIRED ARGS:
$1 should be kubectl version

OPTIONAL ARGS:
-x - kubectx context
-n - kubens namespace

EXAMPLES:
    kver 1.22.9
    kver 1.22.9 -x dev -n app
    kver - # switch to previous version, context, namespace
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
    -add optional -x arg for switching to context  
    -add optional -n arg for switching to namespace  
    -add optional - flag for switching to previous kubectl version, context & namespace  
