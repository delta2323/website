Miscellaneous
=============

Publications
------------

- 2011/11/7 `Jubatus Workshop Tokyo <http://www.zusaar.com/event/165003>`_ (All slide are in Japanese)

 - `"An overview and roadmap of Jubatus" <http://www.slideshare.net/JubatusOfficial/overview-and-roadmap>`_ by Daisuke OKANOHARA
 - `"Feature extraction and liniar classifiers of Jubatus" <http://www.slideshare.net/JubatusOfficial/jubatus-10066854>`_ by Yuya UNNO
 - `"How Jubatus works in Distributed environment" <http://www.slideshare.net/JubatusOfficial/jubatus-workshop>`_ by Kota UENISHI
 - "Jubatus' application and handson" by Satoshi ODA
 - "Estimating nergy consumption using Jubatus" by Shinta NAKAYAMA
 - `"pficommon and MessagePack-RPC" <../_static/tanakh/presen.html>`_ by Hideyuki TANAKA

- 岡野原，他 "大規模分散リアルタイム学習支える技術と今後の展望"， WebDB forum 2011, Tokyo.

- 2011/10/26 Press Relase

 - PFI ( `pfien <http://preferred.jp/2011/10/jubatus-english.html>`_ / `pfija <http://preferred.jp/2011/10/jubatus.html>`_ )
 - NTT ( `nttEN <http://www.ntt.co.jp/news2011/1110e/111026a.html>`_ / `nttJA <http://www.ntt.co.jp/news2011/1110/111026a.html>`_ )
 - `Press Release Slides (in Japanese) <http://www.slideshare.net/JubatusOfficial/jubatus-pressrelease>`_


FAQ
---

- Failed in ``./waf configre`` with ...

::

  ...
  line 298, in load_tool
       __import__(d)
     File "/Users/oliner/tmp/jubatus/unittest_gtest.py", line 8
       C1 = b'#XXX'
                ^
  SyntaxError: invalid syntax

This error occurs when old python. Use python 2.7 or later.

- When using python client, "got socket.error: [Errno 99] Cannot assign requested address" (or kind of `EADDRINUSE`)

 - sudo /sbin/sysctl -w net.ipv4.tcp_tw_recycle=1

- mecab_splitter.trivial and mecab_splitter_create.trivial does not pass the unittest?

 - check your mecab dictionary and ensure that your mecab command accept UTF-8 charsets.

- How does 'jubatus' read?

 - Please do not run 'say' command in MacOS.



Contributions (Thanks a lot!)
-----------------------------

- `MacPorts <http://d.hatena.ne.jp/hjym_u/20111107/1320647557>`_
- `Homebrew <http://d.hatena.ne.jp/katsyoshi/20111107/1320678982>`_

- 0.1.0

 - `Ruby Client <https://github.com/pfi/jubatus-ruby-client>`_
 - `PHP Client <http://d.hatena.ne.jp/oxalis-gps/20111101/1320112193>`_ ( `github repo <https://github.com/oxalis-gps/jubatus-php-client>`_ )
