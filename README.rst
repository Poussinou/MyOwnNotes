**********
MyOwnNotes
**********
Android App for the `ownCloud Notes App`_. Uses the (RESTful) `API of ownCloud notes`_.


The right README
================
Make sure you read the README of the appropriate branch. The one you are seeing right now might not be the one you are looking for.


Contribute
==========
**Use the development branch** and please take a look at CONTRIBUTING.rst for information regarding extending this application.

The information there applies to **translations** and **issue submissions** as well.


Install
=======
to use this app you will need:

+ ownCloud server Version >= 8.0 see `ownCloud Docs`_
+ `ownCloud Notes App`_ Version = 1.0 installed and activated on your server
+ Mobile device using Android Version >= 5 (Lollipop)
+ SSL certificate for your server. For more information please read the `FAQ`_ below.
+ The `My Own Notes App`_ 


.. _`FAQ`:

FAQ
===

What's it with "Installing ownCloud Notes app: No app name specified"?
----------------------------------------------------------------------
the app name as specified in info.xml of the notes app was not exactly the same as the directory name I was using for the app. This happens a lot when unzipping the file downloaded from github. Just rename notes-x.x to notes.

How do I get ownCloud?
----------------------
There are many resources on the internet, showing you how to run your own copy of ownCloud. The following article provides a quick roundup: https://blog.entwicklerbier.org/2014/06/setting-up-owncloud-on-speed/

I get a JSON error - what do I do?
----------------------------------
Please make sure you installed `ownCloud Notes App Version 1.0`_.

I can't connect. Do I really have to use SSL/TLS?
-------------------------------------------------
Short answer: yes. Please read our comment on `Entwicklerbier.org`_ for more information.

I can't connect via SSL. How do I add (self-signed) certificates?
-----------------------------------------------------------------
Use the android Security Settings to add self-signed certificates. Open your Settings, browse to Security and add them there. You can find more information on our `My Own Notes Website`_ and at `google dev`_.

If you are having troubles, please read `Issue #112`_.

If you still need help, feel free to `contact us`_. Please be aware that this mailadress changes as we want to keep spam to a minimum and that it may take a while for us to help out.

I heard you don't support ownCloud's encryption app. Is this true?
------------------------------------------------------------------
Since ownCloud 7.0.4, MyOwnNotes is working with the encryption plugin enabled. However, please look at `our blog entry about ownCloud's encryption app`_ and at `our comment in issue #9392`_ 

Do you know any cheap SSL certificates?
---------------------------------------
Best option is to use `Let's Encrypt`_.

You can also get one for free (for non-profit purposes only) at `StartSSL`_. If you can spend money, we suggest you to take a look at `CheapSSLsecurity`_. Please note that we are not affiliated with those companies in any way. We just want to help you finding cheap certificates.

I have my own certificate. However, it is not working.
------------------------------------------------------
One of the most common errors is a wrong certificate chain. Please use `SSL Labs`_ to check if your certificate chain is in order. If it isn't look up the manual of your webserver. We also wrote an article for `Setting up owncloud on Speed`_. Additionally, please make sure you understand how Android handles SSL certificates. We published relevant information in `Issue #112`_.

I want to move my certificate to a custom folder
------------------------------------------------
Moving certificates can be tedious and insecure, depending on your selinux settings. We do not recommend you to move your certificates. If you are really sure you want to do it, github user `eephyne`_ documented a way to achieve this here: `Moving Certificates`_
Oh, and by the way: Disabling selinux is a really bad idea. Only disable for testing purposes or if you know what you are doing (preferably both :))


Building the application
========================

Starting with MyOwnNotes 2.0 we are using Android Studio. Building information follows soon (tm)...


Contributors
============

Here is a list of all contributers, including ourselves. A big thank you to all the people who help developing this application. Please be aware that all contributions are GPL3 licensed.

Maintainer
----------
* `aykit`_ : Non-profit organisation supporting art, culture and science

Developers
----------
* Main Developer: `steppenhahn`_ 

Translators
-----------
* Basque: `natxooy`_
* English: `aykit`_
* German: `aykit`_ , `kriztan`_
* French: `flo1`_ , `gityeti`_ , `Bonbadil`_ , `dyze`_
* Italian: `valerio-bozzolan`_
* Serbian: `pejakm`_
* Spanish: `tmelikoff`_ , `Roboe`_
* Turkish: `wakeup`_

3rd Party Code
--------------
* `rigrig`_: `PR #108`_

Testers
-------
Unfortunately, we are not able to greet everyone in person. Without your feedback, we wouldn't be able to improve My Own Notes. Please keep up testing and providing valuable information regarding your issues. We promise we will keep up fixing and improving as best as we can.


License
=======
My Own Notes and all contributions are licensed as `GPL3`_ 

.. _API of ownCloud notes: https://github.com/owncloud/notes/wiki/API-0.2
.. _CheapSSLsecurity: https://cheapsslsecurity.com
.. _contact us: mailto:z-o48hohw4l9qla@ay.vc
.. _Entwicklerbier.org: https://blog.entwicklerbier.org/2014/05/securing-the-internet-of-things-how-about-securing-the-internet-first/
.. _google dev: https://code.google.com/p/android/issues/detail?id=11231#c107
.. _GPL3: https://github.com/aykit/myownnotes-android/blob/master/LICENSE
.. _Issue #112: https://github.com/aykit/MyOwnNotes/issues/112
.. _Let's Encrypt: http://letsencrypt.org
.. _Moving Certificates: https://github.com/aykit/myownnotes-android/issues/72
.. _My Own Notes App: https://github.com/aykit/myownnotes
.. _ownCloud Notes App Version 1.0: https://github.com/owncloud/notes/tree/1.0.0
.. _My Own Notes Website: https://aykit.org/sites/myownnotes.html
.. _our blog entry about ownCloud's encryption app: https://blog.entwicklerbier.org/2014/09/misconceptions-of-owncloud-encryption/
.. _our comment in issue #9392: https://github.com/owncloud/core/issues/9392#issuecomment-56274074
.. _ownCloud Docs: http://doc.owncloud.org/
.. _ownCloud Notes App: https://github.com/owncloud/notes
.. _SSL Labs: https://www.ssllabs.com/ssltest/
.. _StartSSL: https://startssl.com
.. _Setting up owncloud on Speed: https://blog.entwicklerbier.org/2014/06/setting-up-owncloud-on-speed/

.. People
.. _aykit: https://aykit.org
.. _Bonbadil: https://github.com/bonbadil
.. _dyze: https://github.com/dyze
.. _eephyne: https://github.com/eephyne
.. _flo1: http:// https://github.com/flo1
.. _gityeti: https://github.com/gityeti
.. _kriztan: https://github.com/kriztan
.. _natxooy: https://github.com/natxooy
.. _pejakm: https://github.com/pejakm
.. _rigrig: 
.. _Roboe: https://github.com/roboe
.. _steppenhahn: https://github.com/steppenhahn
.. _tmelikoff: http://https://github.com/tmelikoff
.. _valerio-bozzolan: https://github.com/valerio-bozzolan
.. _wakeup: https://github.com/wakeup

.. PRs
.. _PR #108: https://github.com/aykit/MyOwnNotes/pull/108
