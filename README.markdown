# Daniel Schildt's vCard Site

It's like a business card!  On the internet!  Oh how _exciting_.

This is forked version mostly based on [Mike West's vCard Site](https://github.com/mikewest/vCard)



## Build

Run `rake` in the project's root directory to compress the PNG files and 
embed them in `./src/index.html` as `data:` URLs.  The result will be
written to `./build/index.html`.


## Offline cache
manifesto generates an HTML5 cache manifest for offline application caching




## Requirements ##

* [Ruby][] version: 1.8.7+
* [manifesto][] version: 1.8.7+

Installing gems:
    [sudo] gem install manifesto


* [OptiPNG][] version: 0.6.5+

Installing with [Homebrew][] on OS X:
	brew install optipng







[ruby]:			http://www.ruby-lang.org/en/						"Ruby Programming Language"
[manifesto]:	http://https://github.com/johntopley/manifesto/		"manifesto generates an HTML5 cache manifest for offline application caching"


[homebrew]:		http://mxcl.github.com/homebrew/					"Homebrew: The missing package manager for OS X"
[optipng]:		http://optipng.sourceforge.net/						"OptiPNG: Advanced PNG Optimizer"


[autiomaa]:		http://autiomaa.org									"Daniel Schildt"
