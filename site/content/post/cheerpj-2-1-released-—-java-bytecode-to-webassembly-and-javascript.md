---
title: CheerpJ 2.1 released — Java bytecode to WebAssembly and JavaScript
date: 2020-06-01T04:33:33.387Z
description: Today we release CheerpJ 2.1, the latest major update to our Java
  to WebAssembly and JavaScript compiler.
image: img/0_-jrisva9ldebptsc.jpeg
---
# About CheerpJ

CheerpJ is a solution to compile ahead of time and execute Java bytecode on the browser in WebAssembly and JavaScript. It comes with a full Java runtime environment, and with Java-JavaScript bidirectional interoperability. CheerpJ provides several browser-based system functions, including virtualized file systems, I/O, networking and audio.

Since release 2.0, CheerpJ supports WebAssembly in its runtime environment, for higher performance and smaller footprint. The full release notes for CheerpJ 2.0 can be found[here](https://medium.com/leaningtech/cheerpj-2-0-released-381f6d03e4e).

# What’s new

CheerpJ 2.1 is a maintenance release introducing several optimizations, bug fixes, and further extending the support for JavaScript interoperability.

New**optimizations**have been introduced in Java exception handling, which are now compiled to much more efficient JavaScript code. Native Java reflection calls — fully supported by CheerpJ — have also been optimized significantly, lowering the overhead in comparison with standard Java calls. We have continued reducing the build size of CheerpJ ahead-of-time JavaScript output.

Improvements to`--stub-natives`, a`cheerpjfy.py`option, allow CheerpJ to create stub JavaScript files for native methods. This allows to develop your own browser-based implementations of native methods in JavaScript/WebAssembly.

Several improvements to the**robustness**of the CheerpJ ahead-of-time compiler, as well as in the Java-JavaScript interoperability, have been introduced.

# Getting started

CheerpJ 2.1 is [available](https://www.leaningtech.com/pages/cheerpj.html#Download) for Windows, macOS and Linux.

**Download and try CheerpJ 2.1**

To try out or update to CheerpJ 2.1, simply download the compiler[here](https://www.leaningtech.com/pages/cheerpj.html), and rebuild your project with the new compiler. If using the CheerpJ cloud runtime, make sure to change your CheerpJ runtime header to:

```
<script src=”https://cjrtnc.leaningtech.com/2.1/loader.js"></script>
```

**Documentation**

You can find the Documentation for CheerpJ, together with tutorials and examples, on the[CheerpJ Documentation](https://leaningtech.com/pages/cheerpj.html#Documentation)page.

# Get in touch!

To report any issues, please use our[issue tracker](https://github.com/leaningtech/cheerpj-meta/issues). For any question or comment, you can find us on the CheerpJ[Gitter channel](https://gitter.im/leaningtech/cheerpj).

Thank you!

Leaning Technologies