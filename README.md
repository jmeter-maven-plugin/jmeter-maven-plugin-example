# Overview #

This is an example project for running a [JMeter ][1]test with the [JMeter Maven Plugin][2] out of the box.

It runs a JMeter test against a few URLs on www.mozilla.com and illustrates how the maven plugin can be used to run
with different configurations, for example a "warmup" and a "real" test.

Included is a JMeter Testplan `test.jmx` that supports 4 distinct threadgroups which can be configured individually.

## Usage ##

  * Execute `mvn verify -Pperformance`
  * look in `target/jmeter/report/` for the JMeter results file and the report

## URL lists ##

The URLs in the file `urls.txt` have to be relative to the hostname.

You could use a website crawler/broken link checker to generate a URL list for your test content. Possible tools:

 * Windows/Linux (using Wine): [Xenu's link sleuth][3]
 * Mac OSX: [Integrity][4]



[1]:    http://jmeter.lazerycode.com                                "JMeter Maven Plugin"
[2]:    http://jakarta.apache.org/jmeter/                           "JMeter"
[3]:    http://home.snafu.de/tilman/xenulink.html                   "Xenu's link sleuth"
[4]:    http://peacockmedia.co.uk/integrity/                        "Integrity"
