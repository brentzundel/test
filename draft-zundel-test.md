---
title: "draft-zundel-test"
category: info

docname: draft-zundel-test-latest
submissiontype: IETF  # also: "independent", "editorial", "IAB", or "IRTF"
number:
date:
consensus: true
v: 3
# area: AREA
# workgroup: WG Working Group
keyword:
 - next generation
 - unicorn
 - sparkling distributed ledger
venue:
#  group: WG
#  type: Working Group
#  mail: WG@example.com
#  arch: https://example.com/WG
  github: "brentzundel/test"
  latest: "https://brentzundel.github.io/test/draft-zundel-test.html"

author:
 -
    fullname: "Brent Zundel"
    organization: Your Organization Here
    email: "brent.zundel@gmail.com"

normative:

informative:

...

--- abstract

TODO Abstract


--- middle

# Introduction

TODO Introduction


# Conventions and Definitions

{::boilerplate bcp14-tagged}

## Direct Presentation Flow
~~~ aasvg

                    +-------+                        +--------+                                              +------+                            +--------+           +---------+
                    |Subject|                        |Mediator|                                              |Issuer|                            |Verifier|           |Presenter|
                    +---+---+                        +----+---+                                              +---+--+                            +----+---+           +----+----+
                        |                                 |                                                      |                                    |                    |
          +-----------+-+---------------------------------+------------------------------------------------------+------------------------------------+--+                 |
          | ISSUANCE  | |                                 |                                                      |                                    |  |                 |
          +-----------+ |<<initiate credential request>>  |                                                      |                                    |  |                 |
          |             +-------------------------------->|                                                      |                                    |  |                 |
          |             |                                 |                                                      |                                    |  |                 |
          |             |                                 |                  request credential                  |                                    |  |                 |
          |             |                                 +----------------------------------------------------->|                                    |  |                 |
          |             |                                 |                                                      |                                    |  |                 |
          |             |                                 |                                                      +------+                             |  |                 |
          |             |                                 |                                                      |      | <<generate credential>>     |  |                 |
          |             |                                 |                                                      |<-----+                             |  |                 |
          |             |                                 |                                                      |                                    |  |                 |
          |             |                                 |                     credential                       |                                    |  |                 |
          |             |                                 |<-----------------------------------------------------+                                    |  |                 |
          +-------------+---------------------------------+------------------------------------------------------+------------------------------------+--+                 |
                        |                                 |                                                      |                                    |                    |
                        |                                 |                                                      |                                    |                    |
                        |               +---------------+-+------------------------------------------------------+------------------------------------+--------------------+--------------+
                        |               | VERIFICATION  | |                                                      |                                    |                    |              |
                        |               +---------------+ |                                                      |            request presentation    |                    |              |
                        |               |                 |<------------------------------------------------------------------------------------------+                    |              |
                        |               |                 |                                                      |                                    |                    |              |
                        |               |                 |             <<prompt to select credential(s)>>       |                                    |                    |              |
                        |               |                 +--------------------------------------------------------------------------------------------------------------->|              |
                        |               |                 |                                                      |                                    |                    |              |
                        |               |                 |            <<select claims from credential(s)>>      |                                    |                    |              |
                        |               |                 |<---------------------------------------------------------------------------------------------------------------+              |
                        |               |                 |                                                      |                                    |                    |              |
                        |               |                 +-----+                                                |                                    |                    |              |
                        |               |                 |     |<<generate presentation proof selection>>       |                                    |                    |              |
                        |               |                 |<----+                                                |                                    |                    |              |
                        |               |                 |                                                      |                                    |                    |              |
                        |               |                 |                                  presentation proof  |                                    |                    |              |
                        |               |                 +------------------------------------------------------------------------------------------>|                    |              |
                        |               +-----------------+------------------------------------------------------+------------------------------------+--------------------+--------------+
                    +---+---+                        +----+---+                                              +---+--+                            +----+---+           +----+----+
                    |Subject|                        |Mediator|                                              |Issuer|                            |Verifier|           |Presenter|
                    +-------+                        +--------+                                              +------+                            +--------+           +---------+
~~~


# Security Considerations

TODO Security


# IANA Considerations

This document has no IANA actions.


--- back

# Acknowledgments
{:numbered="false"}

TODO acknowledge.
