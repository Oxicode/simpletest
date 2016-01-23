SimpleTest [![Build Status](https://travis-ci.org/simpletest/simpletest.svg)](https://travis-ci.org/simpletest/simpletest) [![Latest Stable Version](https://img.shields.io/packagist/v/simpletest/simpletest.svg?style=flat-square)](https://packagist.org/packages/simpletest/simpletest) [![Total Downloads](https://img.shields.io/packagist/dt/simpletest/simpletest.svg?style=flat-square)](https://packagist.org/packages/simpletest/simpletest) [![Latest Unstable Version](https://poser.pugx.org/simpletest/simpletest/v/unstable)](https://packagist.org/packages/simpletest/simpletest) 
==========

SimpleTest is a framework for unit testing, web site testing and
mock objects for PHP.

### Installation

#### Downloads

All downloads are stored on Github Releases.

You may find the zip of the "latest released/tagged version" here:

https://github.com/simpletest/simpletest/releases/latest

You may find the zip archive of the "dev-master" branch here:

https://github.com/simpletest/simpletest/archive/master.zip

#### Composer

You may also install the extension through Composer into the `/vendor` folder of your project.

Either run

    php composer.phar require --prefer-dist simpletest/simpletest "^1.1"

or add

    "simpletest/simpletest": "^1.1"

to the require section of your `composer.json` file, followed by running `composer install`.

### Issues

Please report all issues you encounter over at Github Issues:

https://github.com/simpletest/simpletest/issues

-----

You probably got this package from:

    http://simpletest.org/en/download.html

SimpleTest is a framework for unit testing, web site testing and
mock objects for PHP 5.0.5+.

If you have used JUnit, you will find this PHP unit testing version very
similar. Also included is a mock objects and server stubs generator.
The stubs can have return values set for different arguments, can have
sequences set also by arguments and can return items by reference.
The mocks inherit all of this functionality and can also have
expectations set, again in sequences and for different arguments.

A web tester similar in concept to JWebUnit is also included. There is no
JavaScript or tables support, but forms, authentication, cookies and
frames are handled.

You can see a release schedule at http://simpletest.org/en/overview.html
which is also copied to the documentation folder with this release.
A full PHPDocumenter API documentation exists at
http://simpletest.org/api/.

The user interface is minimal in the extreme, but a lot of information
flows from the test suite. After version 1.0 we will release a better
web UI, but we are leaving XUL and GTK versions to volunteers as
everybody has their own opinion on a good GUI, and we don't want to
discourage development by shipping one with the toolkit. You can
download an Eclipse plug-in separately.

The unit tests for SimpleTest itself can be run here:

    test/unit_tests.php

And tests involving live network connections as well are here:

    test/all_tests.php

The full tests will typically overrun the 8Mb limit often allowed
to a PHP process. A workaround is to run the tests on the command
with a custom php.ini file or with the switch -dmemory_limit=-1
if you do not have access to your server version.

The full tests read some test data from simpletest.org. If the site
is down or has been modified for a later version then you will get
spurious errors. A unit_tests.php failure on the other hand would be
very serious. Please notify us if you find one.

Even if all of the tests run please verify that your existing test suites
also function as expected. The file:

    HELP_MY_TESTS_DONT_WORK_ANYMORE

...contains information on interface changes. It also points out
deprecated interfaces, so you should read this even if all of
your current tests appear to run.

There is a documentation folder which contains the core reference information
in English and French, although this information is fairly basic.
You can find a tutorial on...

    http://simpletest.org/en/first_test_tutorial.html

...to get you started and this material will eventually become included
with the project documentation. A French translation exists at:

    http://simpletest.org/fr/first_test_tutorial.html

If you download and use, and possibly even extend this tool, please let us
know. Any feedback, even bad, is always welcome and we will work to get
your suggestions into the next release. Ideally please send your
comments to:

    simpletest-support@lists.sourceforge.net

...so that others can read them too. We usually try to respond within 48
hours.

There is no change log except at Sourceforge. You can visit the
release notes to see the completed TODO list after each cycle and also the
status of any bugs, but if the bug is recent then it will be fixed in SVN only.
The SVN check-ins always have all the tests passing and so SVN snapshots should
be pretty usable, although the code may not look so good internally.

Oh, and one last thing: SimpleTest is called "Simple" because it should
be simple to use. We intend to add a complete set of tools for a test
first and "test as you code" type of development. "Simple" does not mean
"Lite" in this context.

Thanks to everyone who has sent comments and offered suggestions. They
really are invaluable, but sadly you are too many to mention in full.
Thanks to all on the advanced PHP forum on SitePoint, especially Harry
Fuecks. Early adopters are always an inspiration.

 -- Marcus Baker, Jason Sweat, Travis Swicegood, Perrick Penet and Edward Z. Yang.
