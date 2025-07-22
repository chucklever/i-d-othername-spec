---
title: "Remote Procedure Call Identity Squashing via x.509 Certificate Fields"
abbrev: "SunRPC x.509 Identity Squashing"
category: std

docname: draft-cel-nfsv4-othername-spec-latest
pi: [toc, sortrefs, symrefs, docmapping]
stand_alone: yes
v: 3

submissiontype: IETF
ipr: trust200902
area: "Web and Internet Transport"
workgroup: "Network File System Version 4"
obsoletes:
keyword:
 - x.509
 - SubjectAltName
 - OtherName
 - NFS
 - SunRPC

author:
 -
    fullname: Rick Macklem
    organization: FreeBSD Project
    abbrev: FreeBSD
    country: Canada
    email: rmacklem@uoguelph.ca
 -
    fullname: Chuck Lever
    role: editor
    organization: Oracle Corporation
    abbrev: Oracle
    country: United States of America
    email: chuck.lever@oracle.com

venue:
  group: nfsv4
  type: Working Group
  mail: nfsv4@ietf.org
  arch: https://mailarchive.ietf.org/arch/browse/nfsv4/
  repo: https://github.com/chucklever/i-d-othername-spec
  latest: https://chucklever.github.io/i-d-othername-spec/#go.draft-cel-nfsv4-othername-spec.html

--- abstract

This document extends RPC-with-TLS, as described in {{RFC9289}}, so
that a client's x.509 certificate may carry instructions to the RPC
server to execute all RPC transactions from that client as a single
user identity.

--- middle

# Introduction

## Background

## Problem Statement

## Summary of Proposed Solution

## Open Questions

# Requirements Language

{::boilerplate bcp14-tagged}

# Requirement for OtherName OID

Summary of guidelines regarding use of x.509 SubjectAltName field.
Does this proposal follow those guidelines?

# Format of New OtherName Blob

Follow recommendations of draft-ietf-nfsv4-internationalization-latest
to form an internationalized "user@domain" string similar to NFSv4 ID
map strings.

# Implementation Status

{:aside}
> This section is to be removed before publishing this document as an RFC.

This section records the status of known implementations of the
protocol defined by this specification at the time of posting of this
Internet-Draft, and is based on a proposal described in
{{!RFC7942}}. The description of implementations in this section is
intended to assist the IETF in its decision processes in progressing
drafts to RFCs.

Please note that the listing of any individual implementation here
does not imply endorsement by the IETF. Furthermore, no effort has
been spent to verify the information presented here that was supplied
by IETF contributors. This is not intended as, and must not be
construed to be, a catalog of available implementations or their
features. Readers are advised to note that other implementations may
exist.

## FreeBSD NFS Server and Client

Organization: FreeBSD

URL:       <https://www.freebsd.org>

Maturity:  Complete.

Coverage:  All procedures are implemented.

Licensing: BSD 3-clause

Implementation experience:

# Security Considerations

# IANA Considerations

Request for allocation of a SubjectAltName : OtherName object identifier

--- back

# Acknowledgments
{:numbered="false"}

The authors are grateful to Bill Baker, Jeff Layton, Greg Marsden,
and Martin Thomson for their input and support.

Special thanks to
Area Director
Gorry Fairhurst,
NFSV4 Working Group Chairs
Brian Pawlowski
and
Christopher Inacio,
and
NFSV4 Working Group Secretary
Thomas Haynes
for their guidance and oversight.
