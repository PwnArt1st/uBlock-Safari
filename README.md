<h1>uBlock:</h1><strong> an efficient blocker extension for your browser. Fast, potent, and lean.</strong>


* [Getting Started & Installation](#getting-started)
* [Performance & Benchmarks](#performance)
* [Tips](#tips)
* [About](#about-ublock)

## Getting started

<strong>THIS IS A CUSTOM BUILD OF uBlock THAT MAY OR MAY NOT BE UPDATED.</strong>
<strong>I RECOMMEND YOU USE uBlock Origin IF YOU CAN, OR <a href="https://raw.githubusercontent.com/chrisaljoudi/uBlock/">chrisaljoudi's uBlock</a> INSTEAD</strong>

#### Installation:

<strong> Just a final reminder, this is not for the non tech-savvy, if you dont know what you're doing, stick with whatever is in your browser's app store.</strong>

Now that that's out of the way, to install you can either run `git clone https://github.com/PwnArt1st/uBlock.git` or hit download zip.
Next you will need to `cd` to wherever you downloaded it to, then run `chmod +x tools/make-*your browser*.sh` to make sure the script is executable.
Finally, run `tools/make-*your browser*.sh` to build the extension, which depending on your browser, you can find how to install yourself. The extension will be built into `dist/`.

uBlock has tooltips throughout its UI to help you along. But just in case you need it, [here's a quick guide for basic usage](https://github.com/chrisaljoudi/uBlock/wiki/Quick-guide:-popup-user-interface).

## Performance

#### Memory

<p align="center">
On average, uBlock <b>really</b> does make your browser run leaner. <sup>[1]</sup><br><br>

Chrome <br>
<img src="https://raw.githubusercontent.com/chrisaljoudi/uBlock/master/doc/benchmarks/mem-usage-overall-chart-20141224.png" /><br><br>

Safari<br>
<img src="https://raw.githubusercontent.com/chrisaljoudi/uBlock/master/doc/benchmarks/mem-usage-overall-chart-safari-20150205.png" /><br><br>

Firefox<br>
<img src="https://raw.githubusercontent.com/chrisaljoudi/uBlock/master/doc/benchmarks/mem-usage-overall-chart-20150205.png" /><br><br>

</p>

<sup>[1] An overview of the benchmark is available at <a href="https://github.com/chrisaljoudi/uBlock/wiki/Benchmarking-memory-footprint">this wiki page</a>.</sup><br>

#### CPU

<p align="center">
uBlock is also CPU-efficient<br>
<img src="https://raw.githubusercontent.com/chrisaljoudi/uBlock/master/doc/benchmarks/cpu-usage-overall-chart-20141226.png" /><br>
<sup>Details of the benchmark available in <a href="https://github.com/chrisaljoudi/uBlock/blob/master/doc/benchmarks/cpu-usage-overall-20141226.ods">this LibreOffice spreadsheet</a>.</sup>
</p>

#### Blocking

<p align="center">
Being lean and efficient doesn't mean blocking less<br>
<img src="https://raw.githubusercontent.com/chrisaljoudi/uBlock/master/doc/benchmarks/privex-201502-16.png" /><br>
<sup>For details of benchmark, see 
<a href="https://github.com/chrisaljoudi/uBlock/wiki/uBlock-and-others%3A-Blocking-ads%2C-trackers%2C-malwares">uBlock and others: Blocking ads, trackers, malwares</a>.
</p>

**Some quick tests:**

<sub>These tests are by no means complete or comprehensive, but do remain helpful.</sub>

- [Index](http://raymondhill.net/ublock/tests.html)
- [Web page components](http://raymondhill.net/ublock/tiles1.html)
- [Popups](http://raymondhill.net/ublock/popup.html)

## Tips

* **To benefit from uBlock's higher efficiency,** it's advised that you don't use other inefficient blockers at the same time (such as AdBlock or Adblock Plus). uBlock will do [as well or better](#blocking) than most popular ad blockers.

* It's important to note that blocking ads [is *not* theft](https://twitter.com/LeaVerou/status/518154828166725632). Don't fall for this creepy idea. The _ultimate_ logical consequence of `blocking = theft` is the criminalisation of the inalienable right to privacy.

* _EasyList_, _Peter Lowe's Adservers_, _EasyPrivacy_ and _Malware domains_ are enabled by default when you install uBlock. Many more lists are readily available to block trackers, analytics, and more. Hosts files are also supported.

* Once you install uBlock, you can easily un-select any of the pre-selected filter lists if you think uBlock blocks too much. For reference, Adblock Plus installs with only _EasyList_ enabled by default.

* Feel free to read [about the extension's required permissions](https://github.com/chrisaljoudi/uBlock/wiki/About-the-required-permissions).

## About uBlock



uBlock is a general-purpose blocker — not an *ad blocker* specifically. uBlock's main goal is to help users neutralize privacy-invading apparatus — ads being one example.

uBlock blocks ads through its support of the [Adblock Plus filter syntax](https://adblockplus.org/en/filters). uBlock [extends](https://github.com/chrisaljoudi/uBlock/wiki/Filter-syntax-extensions) the syntax and is designed to work with custom rules and filters.

Free and open-source. For users, by users.

*Acknowledgment:* uBlock comes with several filter lists ready to use out-of-the-box (including but not limited to: EasyList, Peter Lowe's, several malware filter lists). We deeply appreciate the people working hard to maintain those lists which are available to use by all for free.