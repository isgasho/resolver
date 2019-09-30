resolver
============

.. contents::


测试
--------

.. code:: bash
    
    cargo run --example dig baidu.com
    cargo run --example dig 互联网中心.中国


疑问
-------

关于 对 Label 压缩方式，不太确定 LabelPointer 和 LabelString 是否可以混排。

目前看起来有些 DNS 服务器是不支持混排的。

如果有对这个细节比较了解的可以联系我。


特性
-------
*   支持国际化域名的直接查询 (非 ASCII 域名)
*   初步支持 `DNS Message compression`  (注: 还需要再验证准确性)


感兴趣的实现
------------
*   `[RFC1035] DNS Transport over UDP <https://tools.ietf.org/html/rfc1035>`_
*   `[RFC7766] DNS Transport over TCP <https://tools.ietf.org/html/rfc7766>`_
*   `[RFC2535] DNSSEC <https://tools.ietf.org/html/rfc2535>`_
*   `[RFC7858] DNS over Transport Layer Security (TLS) <https://tools.ietf.org/html/rfc7858>`_
*   `[RFC8484] DNS Queries over HTTPS (DoH) <https://tools.ietf.org/html/rfc8484>`_ ， 兴趣不大
*   `DNSCrypt <https://github.com/DNSCrypt/dnscrypt-protocol>`_

