# cmark.swift

[![Build Status](https://travis-ci.org/czechboy0/cmark.swift.svg?branch=master)](https://travis-ci.org/czechboy0/cmark.swift)
[![Latest Release](https://img.shields.io/github/release/czechboy0/cmark.swift.svg)](https://github.com/czechboy0/cmark.swift/releases/latest)
![Platforms](https://img.shields.io/badge/platforms-Linux%20%7C%20OS%20X-blue.svg)
![Package Managers](https://img.shields.io/badge/package%20managers-SwiftPM-yellow.svg)

[![Blog](https://img.shields.io/badge/blog-honzadvorsky.com-green.svg)](http://honzadvorsky.com)
[![Twitter Czechboy0](https://img.shields.io/badge/twitter-czechboy0-green.svg)](http://twitter.com/czechboy0)

> Swift cmark wrapper for SwiftPM

Very simple Swift wrapper of [cmark](https://github.com/jgm/cmark). Uses a [fork](https://github.com/czechboy0/cmark) of cmark which has been adapted for building with SwiftPM.

# Usage

## markdown -> HTML

```swift
let markdown = "# Hello"
let html = try markdownToHTML(markdown)
print(html) //"<h1>Hello</h1>\n"
```

# Warning
Due to a bug in SwiftPM Xcode generation [SR-2526](https://bugs.swift.org/browse/SR-2526), if you're using this package in Xcode, you'll need to add one more header search path to the ccmark target: `Packages/cmark-0.26.1/Sources/ccmark/include`. After you do, everything should build fine in Xcode.

# Installation

## Swift Package Manager

```swift
.Package(url: "https://github.com/czechboy0/cmark.swift.git", majorVersion: 0, minor: 1)
```

:gift_heart: Contributing
------------
Please create an issue with a description of your problem or open a pull request with a fix.

:v: License
-------
MIT

:alien: Author
------
Honza Dvorsky - https://honzadvorsky.com, [@czechboy0](http://twitter.com/czechboy0)

