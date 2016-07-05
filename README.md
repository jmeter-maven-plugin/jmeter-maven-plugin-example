# JMeter Maven Plugin Example #

[![Join the chat at https://gitter.im/jmeter-maven-plugin/jmeter-maven-plugin](https://badges.gitter.im/jmeter-maven-plugin/jmeter-maven-plugin.svg)](https://gitter.im/jmeter-maven-plugin/jmeter-maven-plugin?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
[![Build Status](https://travis-ci.org/jmeter-maven-plugin/jmeter-maven-plugin-example.svg?branch=master)](https://travis-ci.org/jmeter-maven-plugin/jmeter-maven-plugin-example)

## Overview ##

[![Join the chat at https://gitter.im/jmeter-maven-plugin/jmeter-maven-plugin-example](https://badges.gitter.im/jmeter-maven-plugin/jmeter-maven-plugin-example.svg)](https://gitter.im/jmeter-maven-plugin/jmeter-maven-plugin-example?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

This is an example project for running a [JMeter][1] test with the [JMeter Maven Plugin][2] and the [JMeter Analysis Maven Plugin][2] out of the box.

It runs a [JMeter][1] test against a few URLs on www.mozilla.com and illustrates how the maven plugin can be used to run
with different configurations, for example a "warmup" and a "real" test.

Included is a [JMeter][1] Testplan `test.jmx` that supports 4 distinct threadgroups which can be configured individually.

Look at the included files for further information, the `pom.xml` is fully commented, and the JMeter Testplan `test.jmx` as well.

## Usage ##

  * Execute `mvn verify -Pperformance`
  * look in `target/jmeter/report/` for the JMeter results file
  * look in `target/reports/` for the Report generated by the JMeter Analysis Maven Plugin

## URL lists ##

The URLs in the file `urls.txt` have to be relative to the hostname.

You could use a website crawler/broken link checker to generate a URL list for your test content. Possible tools:

 * Windows/Linux (using Wine): [Xenu's link sleuth][3]
 * Mac OSX: [Integrity][4]

Credits
--------------

Part of the development of this workspace is sponsored by [CoreMedia][5]

[1]:    http://jmeter.lazerycode.com                                "JMeter Maven Plugin"
[2]:    http://jakarta.apache.org/jmeter/                           "JMeter"
[3]:    http://home.snafu.de/tilman/xenulink.html                   "Xenu's link sleuth"
[4]:    http://peacockmedia.co.uk/integrity/                        "Integrity"
[5]:    http://www.coremedia.com                                    "CoreMedia AG"

