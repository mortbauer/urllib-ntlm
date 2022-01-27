# urllib-ntlm (also under python-ntlm on github)
Python library that provides NTLM support, including an authentication handler for urllib2.

This library allows you to retrieve content from (usually corporate) servers protected with windows authentication (NTLM) using the python urllib2.

## Python 3 Support

Only python3 is supported.

# Usage

please see the examples directory.

## Limitations
  * A request using the `HTTPNtlmAuthHandler` has no HTTP status handling, for example: redirects are not handled by the opener, you must check and handle the response yourself.

# Resources

## Original Fork
*  https://github.com/mullender/python-ntlm

## Inspired by
  * [http://sourceforge.net/projects/ntlmaps/ NTLM Authorization Proxy Server]
(Dmitri Rozmanov kindly allowed his code to be redistributed under the LGPL)

The NTLM Authorization Proxy Server can be used to make applications that do not support NTLM proxies use them anyway: "Opens up IIS Proxy Servers using NTLM to non-Microsoft browsers, etc"

In contrast the python-ntlm library is used to make it possible for python code to retrieve content from an NTLM protected server. 

## References
  * [MS-NLMP]: [http://download.microsoft.com/download/a/e/6/ae6e4142-aa58-45c6-8dcf-a657e5900cd3/%5BMS-NLMP%5D.pdf NT LAN Manager (NTLM) Authentication Protocol Specification]
  * [MS-NTHT]: [http://download.microsoft.com/download/a/e/6/ae6e4142-aa58-45c6-8dcf-a657e5900cd3/%5BMS-NTHT%5D.pdf NTLM Over HTTP Protocol Specification]
  * [http://www.blackhat.com/presentations/bh-asia-04/bh-jp-04-pdfs/bh-jp-04-seki.pdf Optimized Attack for NTLM2 Session Response]
