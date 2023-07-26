# Comparing `tmp/dnspython-2.4.0rc1.tar.gz` & `tmp/dnspython-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dnspython-2.4.0rc1.tar", max compression
+gzip compressed data, was "dnspython-2.4.1.tar", max compression
```

## Comparing `dnspython-2.4.0rc1.tar` & `dnspython-2.4.1.tar`

### file list

```diff
@@ -1,239 +1,239 @@
--rw-r--r--   0        0        0     1526 2023-07-04 20:25:17.555883 dnspython-2.4.0rc1/LICENSE
--rw-r--r--   0        0        0     3602 2023-07-04 20:25:17.556125 dnspython-2.4.0rc1/README.md
--rw-r--r--   0        0        0     1663 2023-07-04 20:25:17.556391 dnspython-2.4.0rc1/dns/__init__.py
--rw-r--r--   0        0        0     2275 2023-07-04 20:25:17.556483 dnspython-2.4.0rc1/dns/_asyncbackend.py
--rw-r--r--   0        0        0     8664 2023-07-04 20:25:17.556600 dnspython-2.4.0rc1/dns/_asyncio_backend.py
--rw-r--r--   0        0        0     5247 2023-07-04 20:25:17.556701 dnspython-2.4.0rc1/dns/_ddr.py
--rw-r--r--   0        0        0     2459 2023-07-04 20:25:17.556790 dnspython-2.4.0rc1/dns/_immutable_ctx.py
--rw-r--r--   0        0        0     7838 2023-07-04 20:25:17.556896 dnspython-2.4.0rc1/dns/_trio_backend.py
--rw-r--r--   0        0        0     2794 2023-07-04 20:25:17.556987 dnspython-2.4.0rc1/dns/asyncbackend.py
--rw-r--r--   0        0        0    25994 2023-07-04 20:25:17.557140 dnspython-2.4.0rc1/dns/asyncquery.py
--rw-r--r--   0        0        0    17852 2023-07-04 20:25:17.557283 dnspython-2.4.0rc1/dns/asyncresolver.py
--rw-r--r--   0        0        0    40543 2023-07-04 20:25:17.557492 dnspython-2.4.0rc1/dns/dnssec.py
--rw-r--r--   0        0        0     3978 2023-07-04 20:25:17.557633 dnspython-2.4.0rc1/dns/dnssecalgs/__init__.py
--rw-r--r--   0        0        0     2446 2023-07-04 20:25:17.557734 dnspython-2.4.0rc1/dns/dnssecalgs/base.py
--rw-r--r--   0        0        0     2425 2023-07-04 20:25:17.557827 dnspython-2.4.0rc1/dns/dnssecalgs/cryptography.py
--rw-r--r--   0        0        0     3497 2023-07-04 20:25:17.557918 dnspython-2.4.0rc1/dns/dnssecalgs/dsa.py
--rw-r--r--   0        0        0     3016 2023-07-04 20:25:17.558010 dnspython-2.4.0rc1/dns/dnssecalgs/ecdsa.py
--rw-r--r--   0        0        0     1914 2023-07-04 20:25:17.558097 dnspython-2.4.0rc1/dns/dnssecalgs/eddsa.py
--rw-r--r--   0        0        0     3555 2023-07-04 20:25:17.558185 dnspython-2.4.0rc1/dns/dnssecalgs/rsa.py
--rw-r--r--   0        0        0     1799 2023-07-04 20:25:17.558277 dnspython-2.4.0rc1/dns/dnssectypes.py
--rw-r--r--   0        0        0     3978 2023-07-04 20:25:17.558375 dnspython-2.4.0rc1/dns/e164.py
--rw-r--r--   0        0        0    14004 2023-07-04 20:25:17.558517 dnspython-2.4.0rc1/dns/edns.py
--rw-r--r--   0        0        0     4242 2023-07-04 20:25:17.558637 dnspython-2.4.0rc1/dns/entropy.py
--rw-r--r--   0        0        0     3691 2023-07-04 20:25:17.558728 dnspython-2.4.0rc1/dns/enum.py
--rw-r--r--   0        0        0     5957 2023-07-04 20:25:17.558828 dnspython-2.4.0rc1/dns/exception.py
--rw-r--r--   0        0        0     2750 2023-07-04 20:25:17.558931 dnspython-2.4.0rc1/dns/flags.py
--rw-r--r--   0        0        0     2148 2023-07-04 20:25:17.559029 dnspython-2.4.0rc1/dns/grange.py
--rw-r--r--   0        0        0     1836 2023-07-04 20:25:17.559146 dnspython-2.4.0rc1/dns/immutable.py
--rw-r--r--   0        0        0     5278 2023-07-04 20:25:17.559247 dnspython-2.4.0rc1/dns/inet.py
--rw-r--r--   0        0        0     2064 2023-07-04 20:25:17.559340 dnspython-2.4.0rc1/dns/ipv4.py
--rw-r--r--   0        0        0     6192 2023-07-04 20:25:17.559438 dnspython-2.4.0rc1/dns/ipv6.py
--rw-r--r--   0        0        0    63161 2023-07-04 20:25:17.559712 dnspython-2.4.0rc1/dns/message.py
--rw-r--r--   0        0        0    34424 2023-07-04 20:25:17.559936 dnspython-2.4.0rc1/dns/name.py
--rw-r--r--   0        0        0     4000 2023-07-04 20:25:17.560047 dnspython-2.4.0rc1/dns/namedict.py
--rw-r--r--   0        0        0     9096 2023-07-04 20:25:17.560149 dnspython-2.4.0rc1/dns/nameserver.py
--rw-r--r--   0        0        0    12664 2023-07-04 20:25:17.560268 dnspython-2.4.0rc1/dns/node.py
--rw-r--r--   0        0        0     2730 2023-07-04 20:25:17.560373 dnspython-2.4.0rc1/dns/opcode.py
--rw-r--r--   0        0        0        0 2023-07-04 20:25:17.560394 dnspython-2.4.0rc1/dns/py.typed
--rw-r--r--   0        0        0    51760 2023-07-04 20:25:17.560625 dnspython-2.4.0rc1/dns/query.py
--rw-r--r--   0        0        0     2163 2023-07-04 20:25:17.560743 dnspython-2.4.0rc1/dns/quic/__init__.py
--rw-r--r--   0        0        0     7534 2023-07-04 20:25:17.560862 dnspython-2.4.0rc1/dns/quic/_asyncio.py
--rw-r--r--   0        0        0     5460 2023-07-04 20:25:17.560957 dnspython-2.4.0rc1/dns/quic/_common.py
--rw-r--r--   0        0        0     7608 2023-07-04 20:25:17.561070 dnspython-2.4.0rc1/dns/quic/_sync.py
--rw-r--r--   0        0        0     6255 2023-07-04 20:25:17.561176 dnspython-2.4.0rc1/dns/quic/_trio.py
--rw-r--r--   0        0        0     4156 2023-07-04 20:25:17.561280 dnspython-2.4.0rc1/dns/rcode.py
--rw-r--r--   0        0        0    29557 2023-07-04 20:25:17.561459 dnspython-2.4.0rc1/dns/rdata.py
--rw-r--r--   0        0        0     2984 2023-07-04 20:25:17.561566 dnspython-2.4.0rc1/dns/rdataclass.py
--rw-r--r--   0        0        0    17049 2023-07-04 20:25:17.561718 dnspython-2.4.0rc1/dns/rdataset.py
--rw-r--r--   0        0        0     7339 2023-07-04 20:25:17.561851 dnspython-2.4.0rc1/dns/rdatatype.py
--rw-r--r--   0        0        0     1662 2023-07-04 20:25:17.562039 dnspython-2.4.0rc1/dns/rdtypes/ANY/AFSDB.py
--rw-r--r--   0        0        0     3382 2023-07-04 20:25:17.562157 dnspython-2.4.0rc1/dns/rdtypes/ANY/AMTRELAY.py
--rw-r--r--   0        0        0     1025 2023-07-04 20:25:17.562275 dnspython-2.4.0rc1/dns/rdtypes/ANY/AVC.py
--rw-r--r--   0        0        0     2512 2023-07-04 20:25:17.562393 dnspython-2.4.0rc1/dns/rdtypes/ANY/CAA.py
--rw-r--r--   0        0        0     1226 2023-07-04 20:25:17.562492 dnspython-2.4.0rc1/dns/rdtypes/ANY/CDNSKEY.py
--rw-r--r--   0        0        0     1164 2023-07-04 20:25:17.562586 dnspython-2.4.0rc1/dns/rdtypes/ANY/CDS.py
--rw-r--r--   0        0        0     3534 2023-07-04 20:25:17.562698 dnspython-2.4.0rc1/dns/rdtypes/ANY/CERT.py
--rw-r--r--   0        0        0     1207 2023-07-04 20:25:17.562833 dnspython-2.4.0rc1/dns/rdtypes/ANY/CNAME.py
--rw-r--r--   0        0        0     2440 2023-07-04 20:25:17.562955 dnspython-2.4.0rc1/dns/rdtypes/ANY/CSYNC.py
--rw-r--r--   0        0        0      987 2023-07-04 20:25:17.563082 dnspython-2.4.0rc1/dns/rdtypes/ANY/DLV.py
--rw-r--r--   0        0        0     1151 2023-07-04 20:25:17.563200 dnspython-2.4.0rc1/dns/rdtypes/ANY/DNAME.py
--rw-r--r--   0        0        0     1224 2023-07-04 20:25:17.563311 dnspython-2.4.0rc1/dns/rdtypes/ANY/DNSKEY.py
--rw-r--r--   0        0        0      996 2023-07-04 20:25:17.563418 dnspython-2.4.0rc1/dns/rdtypes/ANY/DS.py
--rw-r--r--   0        0        0     1152 2023-07-04 20:25:17.563504 dnspython-2.4.0rc1/dns/rdtypes/ANY/EUI48.py
--rw-r--r--   0        0        0     1162 2023-07-04 20:25:17.563611 dnspython-2.4.0rc1/dns/rdtypes/ANY/EUI64.py
--rw-r--r--   0        0        0     4434 2023-07-04 20:25:17.563722 dnspython-2.4.0rc1/dns/rdtypes/ANY/GPOS.py
--rw-r--r--   0        0        0     2250 2023-07-04 20:25:17.563835 dnspython-2.4.0rc1/dns/rdtypes/ANY/HINFO.py
--rw-r--r--   0        0        0     3229 2023-07-04 20:25:17.563955 dnspython-2.4.0rc1/dns/rdtypes/ANY/HIP.py
--rw-r--r--   0        0        0     2714 2023-07-04 20:25:17.564091 dnspython-2.4.0rc1/dns/rdtypes/ANY/ISDN.py
--rw-r--r--   0        0        0     1287 2023-07-04 20:25:17.564211 dnspython-2.4.0rc1/dns/rdtypes/ANY/L32.py
--rw-r--r--   0        0        0     1593 2023-07-04 20:25:17.564324 dnspython-2.4.0rc1/dns/rdtypes/ANY/L64.py
--rw-r--r--   0        0        0    12025 2023-07-04 20:25:17.564452 dnspython-2.4.0rc1/dns/rdtypes/ANY/LOC.py
--rw-r--r--   0        0        0     1339 2023-07-04 20:25:17.564550 dnspython-2.4.0rc1/dns/rdtypes/ANY/LP.py
--rw-r--r--   0        0        0      996 2023-07-04 20:25:17.564656 dnspython-2.4.0rc1/dns/rdtypes/ANY/MX.py
--rw-r--r--   0        0        0     1545 2023-07-04 20:25:17.564763 dnspython-2.4.0rc1/dns/rdtypes/ANY/NID.py
--rw-r--r--   0        0        0     1042 2023-07-04 20:25:17.564866 dnspython-2.4.0rc1/dns/rdtypes/ANY/NINFO.py
--rw-r--r--   0        0        0      996 2023-07-04 20:25:17.564973 dnspython-2.4.0rc1/dns/rdtypes/ANY/NS.py
--rw-r--r--   0        0        0     2476 2023-07-04 20:25:17.565080 dnspython-2.4.0rc1/dns/rdtypes/ANY/NSEC.py
--rw-r--r--   0        0        0     4152 2023-07-04 20:25:17.565199 dnspython-2.4.0rc1/dns/rdtypes/ANY/NSEC3.py
--rw-r--r--   0        0        0     2636 2023-07-04 20:25:17.565309 dnspython-2.4.0rc1/dns/rdtypes/ANY/NSEC3PARAM.py
--rw-r--r--   0        0        0     1852 2023-07-04 20:25:17.565419 dnspython-2.4.0rc1/dns/rdtypes/ANY/OPENPGPKEY.py
--rw-r--r--   0        0        0     2562 2023-07-04 20:25:17.565534 dnspython-2.4.0rc1/dns/rdtypes/ANY/OPT.py
--rw-r--r--   0        0        0      998 2023-07-04 20:25:17.565640 dnspython-2.4.0rc1/dns/rdtypes/ANY/PTR.py
--rw-r--r--   0        0        0     2185 2023-07-04 20:25:17.565751 dnspython-2.4.0rc1/dns/rdtypes/ANY/RP.py
--rw-r--r--   0        0        0     4924 2023-07-04 20:25:17.565873 dnspython-2.4.0rc1/dns/rdtypes/ANY/RRSIG.py
--rw-r--r--   0        0        0     1014 2023-07-04 20:25:17.565986 dnspython-2.4.0rc1/dns/rdtypes/ANY/RT.py
--rw-r--r--   0        0        0      222 2023-07-04 20:25:17.566041 dnspython-2.4.0rc1/dns/rdtypes/ANY/SMIMEA.py
--rw-r--r--   0        0        0     3146 2023-07-04 20:25:17.566152 dnspython-2.4.0rc1/dns/rdtypes/ANY/SOA.py
--rw-r--r--   0        0        0     1023 2023-07-04 20:25:17.566254 dnspython-2.4.0rc1/dns/rdtypes/ANY/SPF.py
--rw-r--r--   0        0        0     2531 2023-07-04 20:25:17.566363 dnspython-2.4.0rc1/dns/rdtypes/ANY/SSHFP.py
--rw-r--r--   0        0        0     4932 2023-07-04 20:25:17.566488 dnspython-2.4.0rc1/dns/rdtypes/ANY/TKEY.py
--rw-r--r--   0        0        0      219 2023-07-04 20:25:17.566589 dnspython-2.4.0rc1/dns/rdtypes/ANY/TLSA.py
--rw-r--r--   0        0        0     4751 2023-07-04 20:25:17.566722 dnspython-2.4.0rc1/dns/rdtypes/ANY/TSIG.py
--rw-r--r--   0        0        0     1001 2023-07-04 20:25:17.566839 dnspython-2.4.0rc1/dns/rdtypes/ANY/TXT.py
--rw-r--r--   0        0        0     2922 2023-07-04 20:25:17.566954 dnspython-2.4.0rc1/dns/rdtypes/ANY/URI.py
--rw-r--r--   0        0        0     1945 2023-07-04 20:25:17.567073 dnspython-2.4.0rc1/dns/rdtypes/ANY/X25.py
--rw-r--r--   0        0        0     2394 2023-07-04 20:25:17.567194 dnspython-2.4.0rc1/dns/rdtypes/ANY/ZONEMD.py
--rw-r--r--   0        0        0     1497 2023-07-04 20:25:17.567301 dnspython-2.4.0rc1/dns/rdtypes/ANY/__init__.py
--rw-r--r--   0        0        0     2217 2023-07-04 20:25:17.567452 dnspython-2.4.0rc1/dns/rdtypes/CH/A.py
--rw-r--r--   0        0        0      923 2023-07-04 20:25:17.567576 dnspython-2.4.0rc1/dns/rdtypes/CH/__init__.py
--rw-r--r--   0        0        0     1815 2023-07-04 20:25:17.567726 dnspython-2.4.0rc1/dns/rdtypes/IN/A.py
--rw-r--r--   0        0        0     1821 2023-07-04 20:25:17.567850 dnspython-2.4.0rc1/dns/rdtypes/IN/AAAA.py
--rw-r--r--   0        0        0     5099 2023-07-04 20:25:17.567982 dnspython-2.4.0rc1/dns/rdtypes/IN/APL.py
--rw-r--r--   0        0        0     1857 2023-07-04 20:25:17.568096 dnspython-2.4.0rc1/dns/rdtypes/IN/DHCID.py
--rw-r--r--   0        0        0      220 2023-07-04 20:25:17.568206 dnspython-2.4.0rc1/dns/rdtypes/IN/HTTPS.py
--rw-r--r--   0        0        0     3291 2023-07-04 20:25:17.568324 dnspython-2.4.0rc1/dns/rdtypes/IN/IPSECKEY.py
--rw-r--r--   0        0        0     1014 2023-07-04 20:25:17.568415 dnspython-2.4.0rc1/dns/rdtypes/IN/KX.py
--rw-r--r--   0        0        0     3751 2023-07-04 20:25:17.568541 dnspython-2.4.0rc1/dns/rdtypes/IN/NAPTR.py
--rw-r--r--   0        0        0     2166 2023-07-04 20:25:17.568668 dnspython-2.4.0rc1/dns/rdtypes/IN/NSAP.py
--rw-r--r--   0        0        0     1016 2023-07-04 20:25:17.568778 dnspython-2.4.0rc1/dns/rdtypes/IN/NSAP_PTR.py
--rw-r--r--   0        0        0     2757 2023-07-04 20:25:17.568879 dnspython-2.4.0rc1/dns/rdtypes/IN/PX.py
--rw-r--r--   0        0        0     2770 2023-07-04 20:25:17.568984 dnspython-2.4.0rc1/dns/rdtypes/IN/SRV.py
--rw-r--r--   0        0        0      218 2023-07-04 20:25:17.569089 dnspython-2.4.0rc1/dns/rdtypes/IN/SVCB.py
--rw-r--r--   0        0        0     3653 2023-07-04 20:25:17.569205 dnspython-2.4.0rc1/dns/rdtypes/IN/WKS.py
--rw-r--r--   0        0        0     1083 2023-07-04 20:25:17.569312 dnspython-2.4.0rc1/dns/rdtypes/IN/__init__.py
--rw-r--r--   0        0        0     1073 2023-07-04 20:25:17.569420 dnspython-2.4.0rc1/dns/rdtypes/__init__.py
--rw-r--r--   0        0        0     2857 2023-07-04 20:25:17.569527 dnspython-2.4.0rc1/dns/rdtypes/dnskeybase.py
--rw-r--r--   0        0        0     3428 2023-07-04 20:25:17.569634 dnspython-2.4.0rc1/dns/rdtypes/dsbase.py
--rw-r--r--   0        0        0     2631 2023-07-04 20:25:17.569734 dnspython-2.4.0rc1/dns/rdtypes/euibase.py
--rw-r--r--   0        0        0     3199 2023-07-04 20:25:17.569836 dnspython-2.4.0rc1/dns/rdtypes/mxbase.py
--rw-r--r--   0        0        0     2325 2023-07-04 20:25:17.569936 dnspython-2.4.0rc1/dns/rdtypes/nsbase.py
--rw-r--r--   0        0        0    16952 2023-07-04 20:25:17.570083 dnspython-2.4.0rc1/dns/rdtypes/svcbbase.py
--rw-r--r--   0        0        0     2597 2023-07-04 20:25:17.570192 dnspython-2.4.0rc1/dns/rdtypes/tlsabase.py
--rw-r--r--   0        0        0     3630 2023-07-04 20:25:17.570305 dnspython-2.4.0rc1/dns/rdtypes/txtbase.py
--rw-r--r--   0        0        0     9003 2023-07-04 20:25:17.570427 dnspython-2.4.0rc1/dns/rdtypes/util.py
--rw-r--r--   0        0        0    10673 2023-07-04 20:25:17.570554 dnspython-2.4.0rc1/dns/renderer.py
--rw-r--r--   0        0        0    73514 2023-07-04 20:25:17.570871 dnspython-2.4.0rc1/dns/resolver.py
--rw-r--r--   0        0        0     3828 2023-07-04 20:25:17.570982 dnspython-2.4.0rc1/dns/reversename.py
--rw-r--r--   0        0        0     9168 2023-07-04 20:25:17.571090 dnspython-2.4.0rc1/dns/rrset.py
--rw-r--r--   0        0        0     3606 2023-07-04 20:25:17.571184 dnspython-2.4.0rc1/dns/serial.py
--rw-r--r--   0        0        0     9089 2023-07-04 20:25:17.571296 dnspython-2.4.0rc1/dns/set.py
--rw-r--r--   0        0        0    23583 2023-07-04 20:25:17.571448 dnspython-2.4.0rc1/dns/tokenizer.py
--rw-r--r--   0        0        0    22660 2023-07-04 20:25:17.571593 dnspython-2.4.0rc1/dns/transaction.py
--rw-r--r--   0        0        0    11422 2023-07-04 20:25:17.571716 dnspython-2.4.0rc1/dns/tsig.py
--rw-r--r--   0        0        0     2633 2023-07-04 20:25:17.571812 dnspython-2.4.0rc1/dns/tsigkeyring.py
--rw-r--r--   0        0        0     2979 2023-07-04 20:25:17.571905 dnspython-2.4.0rc1/dns/ttl.py
--rw-r--r--   0        0        0    12243 2023-07-04 20:25:17.572013 dnspython-2.4.0rc1/dns/update.py
--rw-r--r--   0        0        0     1926 2023-07-04 20:25:17.572101 dnspython-2.4.0rc1/dns/version.py
--rw-r--r--   0        0        0    11765 2023-07-04 20:25:17.572210 dnspython-2.4.0rc1/dns/versioned.py
--rw-r--r--   0        0        0     9057 2023-07-04 20:25:17.572313 dnspython-2.4.0rc1/dns/win32util.py
--rw-r--r--   0        0        0     2830 2023-07-04 20:25:17.572408 dnspython-2.4.0rc1/dns/wire.py
--rw-r--r--   0        0        0    13273 2023-07-04 20:25:17.572527 dnspython-2.4.0rc1/dns/xfr.py
--rw-r--r--   0        0        0    51093 2023-07-04 20:25:17.572741 dnspython-2.4.0rc1/dns/zone.py
--rw-r--r--   0        0        0    27930 2023-07-04 20:25:17.572907 dnspython-2.4.0rc1/dns/zonefile.py
--rw-r--r--   0        0        0      690 2023-07-04 20:25:17.573002 dnspython-2.4.0rc1/dns/zonetypes.py
--rw-r--r--   0        0        0      874 2023-07-04 20:25:17.576936 dnspython-2.4.0rc1/examples/async_dns.py
--rwxr-xr-x   0        0        0     1194 2023-07-04 20:25:17.577026 dnspython-2.4.0rc1/examples/ddns.py
--rw-r--r--   0        0        0      950 2023-07-04 20:25:17.577121 dnspython-2.4.0rc1/examples/ddr.py
--rwxr-xr-x   0        0        0     3001 2023-07-04 20:25:17.577215 dnspython-2.4.0rc1/examples/doh-json.py
--rwxr-xr-x   0        0        0      534 2023-07-04 20:25:17.577298 dnspython-2.4.0rc1/examples/doh.py
--rw-r--r--   0        0        0     3143 2023-07-04 20:25:17.577395 dnspython-2.4.0rc1/examples/doq.py
--rwxr-xr-x   0        0        0      115 2023-07-04 20:25:17.577473 dnspython-2.4.0rc1/examples/e164.py
--rwxr-xr-x   0        0        0      427 2023-07-04 20:25:17.577562 dnspython-2.4.0rc1/examples/ecs.py
--rwxr-xr-x   0        0        0     1739 2023-07-04 20:25:17.577656 dnspython-2.4.0rc1/examples/edns.py
--rw-r--r--   0        0        0     1532 2023-07-04 20:25:17.577756 dnspython-2.4.0rc1/examples/edns_resolver.py
--rwxr-xr-x   0        0        0      189 2023-07-04 20:25:17.577853 dnspython-2.4.0rc1/examples/mx.py
--rwxr-xr-x   0        0        0      356 2023-07-04 20:25:17.577945 dnspython-2.4.0rc1/examples/name.py
--rw-r--r--   0        0        0     1655 2023-07-04 20:25:17.578033 dnspython-2.4.0rc1/examples/query_specific.py
--rw-r--r--   0        0        0     1022 2023-07-04 20:25:17.578118 dnspython-2.4.0rc1/examples/receive_notify.py
--rwxr-xr-x   0        0        0     1389 2023-07-04 20:25:17.578204 dnspython-2.4.0rc1/examples/reverse.py
--rwxr-xr-x   0        0        0      140 2023-07-04 20:25:17.578290 dnspython-2.4.0rc1/examples/reverse_name.py
--rwxr-xr-x   0        0        0      340 2023-07-04 20:25:17.578377 dnspython-2.4.0rc1/examples/xfr.py
--rwxr-xr-x   0        0        0    12173 2023-07-04 20:25:17.578484 dnspython-2.4.0rc1/examples/zonediff.py
--rw-r--r--   0        0        0     2202 2023-07-04 20:25:17.578733 dnspython-2.4.0rc1/pyproject.toml
--rw-r--r--   0        0        0     1970 2023-07-04 20:25:17.578869 dnspython-2.4.0rc1/setup.cfg
--rw-r--r--   0        0        0        0 2023-07-04 20:25:17.579110 dnspython-2.4.0rc1/tests/__init__.py
--rw-r--r--   0        0        0    12881 2023-07-04 20:25:17.579239 dnspython-2.4.0rc1/tests/example
--rw-r--r--   0        0        0    11010 2023-07-04 20:25:17.579352 dnspython-2.4.0rc1/tests/example1.good
--rw-r--r--   0        0        0    12699 2023-07-04 20:25:17.579470 dnspython-2.4.0rc1/tests/example2.good
--rw-r--r--   0        0        0    11010 2023-07-04 20:25:17.579582 dnspython-2.4.0rc1/tests/example3.good
--rw-r--r--   0        0        0    11027 2023-07-04 20:25:17.579702 dnspython-2.4.0rc1/tests/example4.good
--rw-r--r--   0        0        0     8696 2023-07-04 20:25:17.579816 dnspython-2.4.0rc1/tests/keys.py
--rw-r--r--   0        0        0       91 2023-07-04 20:25:17.579893 dnspython-2.4.0rc1/tests/md_module.py
--rw-r--r--   0        0        0      223 2023-07-04 20:25:17.579936 dnspython-2.4.0rc1/tests/mx-2-0.pickle
--rw-r--r--   0        0        0    11832 2023-07-04 20:25:17.580050 dnspython-2.4.0rc1/tests/nanonameserver.py
--rw-r--r--   0        0        0     4246 2023-07-04 20:25:17.580145 dnspython-2.4.0rc1/tests/nanoquic.py
--rw-r--r--   0        0        0      140 2023-07-04 20:25:17.580189 dnspython-2.4.0rc1/tests/query
--rw-r--r--   0        0        0      111 2023-07-04 20:25:17.580274 dnspython-2.4.0rc1/tests/stxt_module.py
--rw-r--r--   0        0        0     4573 2023-07-04 20:25:17.580325 dnspython-2.4.0rc1/tests/svcb_test_vectors.generic
--rw-r--r--   0        0        0     1157 2023-07-04 20:25:17.580371 dnspython-2.4.0rc1/tests/svcb_test_vectors.text
--rw-r--r--   0        0        0    21140 2023-07-04 20:25:17.580497 dnspython-2.4.0rc1/tests/test_address.py
--rw-r--r--   0        0        0    23340 2023-07-04 20:25:17.580646 dnspython-2.4.0rc1/tests/test_async.py
--rw-r--r--   0        0        0     3752 2023-07-04 20:25:17.580757 dnspython-2.4.0rc1/tests/test_bugs.py
--rw-r--r--   0        0        0     1295 2023-07-04 20:25:17.580847 dnspython-2.4.0rc1/tests/test_constants.py
--rw-r--r--   0        0        0     1258 2023-07-04 20:25:17.580940 dnspython-2.4.0rc1/tests/test_ddr.py
--rw-r--r--   0        0        0    50033 2023-07-04 20:25:17.581161 dnspython-2.4.0rc1/tests/test_dnssec.py
--rw-r--r--   0        0        0    10264 2023-07-04 20:25:17.581285 dnspython-2.4.0rc1/tests/test_dnssecalgs.py
--rw-r--r--   0        0        0     6976 2023-07-04 20:25:17.581400 dnspython-2.4.0rc1/tests/test_doh.py
--rw-r--r--   0        0        0     1401 2023-07-04 20:25:17.581489 dnspython-2.4.0rc1/tests/test_doq.py
--rw-r--r--   0        0        0     8926 2023-07-04 20:25:17.581597 dnspython-2.4.0rc1/tests/test_edns.py
--rw-r--r--   0        0        0     1977 2023-07-04 20:25:17.581693 dnspython-2.4.0rc1/tests/test_entropy.py
--rw-r--r--   0        0        0     2192 2023-07-04 20:25:17.581783 dnspython-2.4.0rc1/tests/test_exceptions.py
--rw-r--r--   0        0        0     2914 2023-07-04 20:25:17.581875 dnspython-2.4.0rc1/tests/test_flags.py
--rw-r--r--   0        0        0    24372 2023-07-04 20:25:17.581994 dnspython-2.4.0rc1/tests/test_generate.py
--rw-r--r--   0        0        0     3055 2023-07-04 20:25:17.582093 dnspython-2.4.0rc1/tests/test_grange.py
--rw-r--r--   0        0        0     4384 2023-07-04 20:25:17.582189 dnspython-2.4.0rc1/tests/test_immutable.py
--rw-r--r--   0        0        0    27696 2023-07-04 20:25:17.582354 dnspython-2.4.0rc1/tests/test_message.py
--rw-r--r--   0        0        0    37873 2023-07-04 20:25:17.582541 dnspython-2.4.0rc1/tests/test_name.py
--rw-r--r--   0        0        0     5625 2023-07-04 20:25:17.582643 dnspython-2.4.0rc1/tests/test_namedict.py
--rw-r--r--   0        0        0     1907 2023-07-04 20:25:17.582730 dnspython-2.4.0rc1/tests/test_nsec3.py
--rw-r--r--   0        0        0     3685 2023-07-04 20:25:17.582820 dnspython-2.4.0rc1/tests/test_nsec3_hash.py
--rw-r--r--   0        0        0    10872 2023-07-04 20:25:17.582933 dnspython-2.4.0rc1/tests/test_ntoaaton.py
--rw-r--r--   0        0        0     4037 2023-07-04 20:25:17.583042 dnspython-2.4.0rc1/tests/test_processing_order.py
--rw-r--r--   0        0        0    23514 2023-07-04 20:25:17.583177 dnspython-2.4.0rc1/tests/test_query.py
--rw-r--r--   0        0        0    43483 2023-07-04 20:25:17.583386 dnspython-2.4.0rc1/tests/test_rdata.py
--rw-r--r--   0        0        0     6136 2023-07-04 20:25:17.583494 dnspython-2.4.0rc1/tests/test_rdataset.py
--rw-r--r--   0        0        0     4307 2023-07-04 20:25:17.583593 dnspython-2.4.0rc1/tests/test_rdtypeandclass.py
--rw-r--r--   0        0        0     1696 2023-07-04 20:25:17.583681 dnspython-2.4.0rc1/tests/test_rdtypeanydnskey.py
--rw-r--r--   0        0        0     7283 2023-07-04 20:25:17.583782 dnspython-2.4.0rc1/tests/test_rdtypeanyeui.py
--rw-r--r--   0        0        0     3437 2023-07-04 20:25:17.583873 dnspython-2.4.0rc1/tests/test_rdtypeanyloc.py
--rw-r--r--   0        0        0     4309 2023-07-04 20:25:17.583966 dnspython-2.4.0rc1/tests/test_rdtypeanytkey.py
--rw-r--r--   0        0        0     3972 2023-07-04 20:25:17.584071 dnspython-2.4.0rc1/tests/test_renderer.py
--rw-r--r--   0        0        0    21664 2023-07-04 20:25:17.584211 dnspython-2.4.0rc1/tests/test_resolution.py
--rw-r--r--   0        0        0    45216 2023-07-04 20:25:17.584418 dnspython-2.4.0rc1/tests/test_resolver.py
--rw-r--r--   0        0        0     8942 2023-07-04 20:25:17.584540 dnspython-2.4.0rc1/tests/test_resolver_override.py
--rw-r--r--   0        0        0     8220 2023-07-04 20:25:17.584665 dnspython-2.4.0rc1/tests/test_rrset.py
--rw-r--r--   0        0        0     3920 2023-07-04 20:25:17.584771 dnspython-2.4.0rc1/tests/test_rrset_reader.py
--rw-r--r--   0        0        0     3776 2023-07-04 20:25:17.584870 dnspython-2.4.0rc1/tests/test_serial.py
--rw-r--r--   0        0        0     8872 2023-07-04 20:25:17.584980 dnspython-2.4.0rc1/tests/test_set.py
--rw-r--r--   0        0        0    14173 2023-07-04 20:25:17.585109 dnspython-2.4.0rc1/tests/test_svcb.py
--rw-r--r--   0        0        0    13465 2023-07-04 20:25:17.585229 dnspython-2.4.0rc1/tests/test_tokenizer.py
--rw-r--r--   0        0        0    22137 2023-07-04 20:25:17.585383 dnspython-2.4.0rc1/tests/test_transaction.py
--rw-r--r--   0        0        0    12773 2023-07-04 20:25:17.585516 dnspython-2.4.0rc1/tests/test_tsig.py
--rw-r--r--   0        0        0     2072 2023-07-04 20:25:17.585610 dnspython-2.4.0rc1/tests/test_tsigkeyring.py
--rw-r--r--   0        0        0     1120 2023-07-04 20:25:17.585695 dnspython-2.4.0rc1/tests/test_ttl.py
--rw-r--r--   0        0        0    11423 2023-07-04 20:25:17.585807 dnspython-2.4.0rc1/tests/test_update.py
--rw-r--r--   0        0        0     3308 2023-07-04 20:25:17.585909 dnspython-2.4.0rc1/tests/test_wire.py
--rw-r--r--   0        0        0    21524 2023-07-04 20:25:17.586053 dnspython-2.4.0rc1/tests/test_xfr.py
--rw-r--r--   0        0        0    45309 2023-07-04 20:25:17.586257 dnspython-2.4.0rc1/tests/test_zone.py
--rw-r--r--   0        0        0     9119 2023-07-04 20:25:17.586372 dnspython-2.4.0rc1/tests/test_zonedigest.py
--rw-r--r--   0        0        0     1204 2023-07-04 20:25:17.586501 dnspython-2.4.0rc1/tests/tls/ca.crt
--rw-r--r--   0        0        0      119 2023-07-04 20:25:17.586584 dnspython-2.4.0rc1/tests/tls/private.pem
--rw-r--r--   0        0        0     2095 2023-07-04 20:25:17.586681 dnspython-2.4.0rc1/tests/tls/public.crt
--rw-r--r--   0        0        0      101 2023-07-04 20:25:17.586769 dnspython-2.4.0rc1/tests/ttxt_module.py
--rw-r--r--   0        0        0      372 2023-07-04 20:25:17.586854 dnspython-2.4.0rc1/tests/utest.py
--rw-r--r--   0        0        0     4215 2023-07-04 20:25:17.586962 dnspython-2.4.0rc1/tests/util.py
--rwxr-xr-x   0        0        0     3126 2023-07-04 20:25:17.587063 dnspython-2.4.0rc1/util/constants-tool
--rw-r--r--   0        0        0      437 2023-07-04 20:25:17.587148 dnspython-2.4.0rc1/util/generate-mx-pickle.py
--rw-r--r--   0        0        0      358 2023-07-04 20:25:17.587242 dnspython-2.4.0rc1/util/generate-rdatatype-doc.py
--rw-r--r--   0        0        0     4952 1970-01-01 00:00:00.000000 dnspython-2.4.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     1526 2023-07-25 19:11:52.188918 dnspython-2.4.1/LICENSE
+-rw-r--r--   0        0        0     3607 2023-07-25 19:11:59.369879 dnspython-2.4.1/README.md
+-rw-r--r--   0        0        0     1663 2023-07-25 19:11:52.189421 dnspython-2.4.1/dns/__init__.py
+-rw-r--r--   0        0        0     2275 2023-07-25 19:11:52.189516 dnspython-2.4.1/dns/_asyncbackend.py
+-rw-r--r--   0        0        0     8850 2023-07-25 19:11:52.189624 dnspython-2.4.1/dns/_asyncio_backend.py
+-rw-r--r--   0        0        0     5247 2023-07-25 19:11:52.189720 dnspython-2.4.1/dns/_ddr.py
+-rw-r--r--   0        0        0     2459 2023-07-25 19:11:52.189818 dnspython-2.4.1/dns/_immutable_ctx.py
+-rw-r--r--   0        0        0     7887 2023-07-25 19:11:52.189925 dnspython-2.4.1/dns/_trio_backend.py
+-rw-r--r--   0        0        0     2794 2023-07-25 19:11:52.190026 dnspython-2.4.1/dns/asyncbackend.py
+-rw-r--r--   0        0        0    25978 2023-07-25 19:11:52.190192 dnspython-2.4.1/dns/asyncquery.py
+-rw-r--r--   0        0        0    17852 2023-07-25 19:11:52.190344 dnspython-2.4.1/dns/asyncresolver.py
+-rw-r--r--   0        0        0    40664 2023-07-25 19:11:52.190555 dnspython-2.4.1/dns/dnssec.py
+-rw-r--r--   0        0        0     4270 2023-07-25 19:11:52.190688 dnspython-2.4.1/dns/dnssecalgs/__init__.py
+-rw-r--r--   0        0        0     2446 2023-07-25 19:11:52.190785 dnspython-2.4.1/dns/dnssecalgs/base.py
+-rw-r--r--   0        0        0     2425 2023-07-25 19:11:52.190882 dnspython-2.4.1/dns/dnssecalgs/cryptography.py
+-rw-r--r--   0        0        0     3497 2023-07-25 19:11:52.190989 dnspython-2.4.1/dns/dnssecalgs/dsa.py
+-rw-r--r--   0        0        0     3016 2023-07-25 19:11:52.191103 dnspython-2.4.1/dns/dnssecalgs/ecdsa.py
+-rw-r--r--   0        0        0     1914 2023-07-25 19:11:52.191220 dnspython-2.4.1/dns/dnssecalgs/eddsa.py
+-rw-r--r--   0        0        0     3555 2023-07-25 19:11:52.191340 dnspython-2.4.1/dns/dnssecalgs/rsa.py
+-rw-r--r--   0        0        0     1799 2023-07-25 19:11:52.191582 dnspython-2.4.1/dns/dnssectypes.py
+-rw-r--r--   0        0        0     3978 2023-07-25 19:11:52.191802 dnspython-2.4.1/dns/e164.py
+-rw-r--r--   0        0        0    14004 2023-07-25 19:11:52.191942 dnspython-2.4.1/dns/edns.py
+-rw-r--r--   0        0        0     4242 2023-07-25 19:11:52.192052 dnspython-2.4.1/dns/entropy.py
+-rw-r--r--   0        0        0     3691 2023-07-25 19:11:52.192149 dnspython-2.4.1/dns/enum.py
+-rw-r--r--   0        0        0     5957 2023-07-25 19:11:52.192246 dnspython-2.4.1/dns/exception.py
+-rw-r--r--   0        0        0     2750 2023-07-25 19:11:52.192344 dnspython-2.4.1/dns/flags.py
+-rw-r--r--   0        0        0     2148 2023-07-25 19:11:52.192520 dnspython-2.4.1/dns/grange.py
+-rw-r--r--   0        0        0     1836 2023-07-25 19:11:52.192612 dnspython-2.4.1/dns/immutable.py
+-rw-r--r--   0        0        0     5278 2023-07-25 19:11:52.192708 dnspython-2.4.1/dns/inet.py
+-rw-r--r--   0        0        0     2064 2023-07-25 19:11:52.192793 dnspython-2.4.1/dns/ipv4.py
+-rw-r--r--   0        0        0     6192 2023-07-25 19:11:52.192902 dnspython-2.4.1/dns/ipv6.py
+-rw-r--r--   0        0        0    63161 2023-07-25 19:11:52.193170 dnspython-2.4.1/dns/message.py
+-rw-r--r--   0        0        0    34424 2023-07-25 19:11:52.193366 dnspython-2.4.1/dns/name.py
+-rw-r--r--   0        0        0     4000 2023-07-25 19:11:52.193556 dnspython-2.4.1/dns/namedict.py
+-rw-r--r--   0        0        0     9096 2023-07-25 19:11:52.193653 dnspython-2.4.1/dns/nameserver.py
+-rw-r--r--   0        0        0    12664 2023-07-25 19:11:52.193779 dnspython-2.4.1/dns/node.py
+-rw-r--r--   0        0        0     2730 2023-07-25 19:11:52.193897 dnspython-2.4.1/dns/opcode.py
+-rw-r--r--   0        0        0        0 2023-07-25 19:11:52.193916 dnspython-2.4.1/dns/py.typed
+-rw-r--r--   0        0        0    51888 2023-07-25 19:11:52.194152 dnspython-2.4.1/dns/query.py
+-rw-r--r--   0        0        0     2163 2023-07-25 19:11:52.194277 dnspython-2.4.1/dns/quic/__init__.py
+-rw-r--r--   0        0        0     8003 2023-07-25 19:11:52.194383 dnspython-2.4.1/dns/quic/_asyncio.py
+-rw-r--r--   0        0        0     5503 2023-07-25 19:11:52.194479 dnspython-2.4.1/dns/quic/_common.py
+-rw-r--r--   0        0        0     7707 2023-07-25 19:11:52.194580 dnspython-2.4.1/dns/quic/_sync.py
+-rw-r--r--   0        0        0     6544 2023-07-25 19:11:52.194678 dnspython-2.4.1/dns/quic/_trio.py
+-rw-r--r--   0        0        0     4156 2023-07-25 19:11:52.194803 dnspython-2.4.1/dns/rcode.py
+-rw-r--r--   0        0        0    29557 2023-07-25 19:11:52.194965 dnspython-2.4.1/dns/rdata.py
+-rw-r--r--   0        0        0     2984 2023-07-25 19:11:52.195084 dnspython-2.4.1/dns/rdataclass.py
+-rw-r--r--   0        0        0    17049 2023-07-25 19:11:52.195213 dnspython-2.4.1/dns/rdataset.py
+-rw-r--r--   0        0        0     7339 2023-07-25 19:11:52.195402 dnspython-2.4.1/dns/rdatatype.py
+-rw-r--r--   0        0        0     1662 2023-07-25 19:11:52.195554 dnspython-2.4.1/dns/rdtypes/ANY/AFSDB.py
+-rw-r--r--   0        0        0     3382 2023-07-25 19:11:52.195677 dnspython-2.4.1/dns/rdtypes/ANY/AMTRELAY.py
+-rw-r--r--   0        0        0     1025 2023-07-25 19:11:52.195768 dnspython-2.4.1/dns/rdtypes/ANY/AVC.py
+-rw-r--r--   0        0        0     2512 2023-07-25 19:11:52.195888 dnspython-2.4.1/dns/rdtypes/ANY/CAA.py
+-rw-r--r--   0        0        0     1226 2023-07-25 19:11:52.195971 dnspython-2.4.1/dns/rdtypes/ANY/CDNSKEY.py
+-rw-r--r--   0        0        0     1164 2023-07-25 19:11:52.196055 dnspython-2.4.1/dns/rdtypes/ANY/CDS.py
+-rw-r--r--   0        0        0     3534 2023-07-25 19:11:52.196143 dnspython-2.4.1/dns/rdtypes/ANY/CERT.py
+-rw-r--r--   0        0        0     1207 2023-07-25 19:11:52.196228 dnspython-2.4.1/dns/rdtypes/ANY/CNAME.py
+-rw-r--r--   0        0        0     2440 2023-07-25 19:11:52.196315 dnspython-2.4.1/dns/rdtypes/ANY/CSYNC.py
+-rw-r--r--   0        0        0      987 2023-07-25 19:11:52.196403 dnspython-2.4.1/dns/rdtypes/ANY/DLV.py
+-rw-r--r--   0        0        0     1151 2023-07-25 19:11:52.196489 dnspython-2.4.1/dns/rdtypes/ANY/DNAME.py
+-rw-r--r--   0        0        0     1224 2023-07-25 19:11:52.196571 dnspython-2.4.1/dns/rdtypes/ANY/DNSKEY.py
+-rw-r--r--   0        0        0      996 2023-07-25 19:11:52.196656 dnspython-2.4.1/dns/rdtypes/ANY/DS.py
+-rw-r--r--   0        0        0     1152 2023-07-25 19:11:52.196742 dnspython-2.4.1/dns/rdtypes/ANY/EUI48.py
+-rw-r--r--   0        0        0     1162 2023-07-25 19:11:52.196828 dnspython-2.4.1/dns/rdtypes/ANY/EUI64.py
+-rw-r--r--   0        0        0     4434 2023-07-25 19:11:52.196955 dnspython-2.4.1/dns/rdtypes/ANY/GPOS.py
+-rw-r--r--   0        0        0     2250 2023-07-25 19:11:52.197092 dnspython-2.4.1/dns/rdtypes/ANY/HINFO.py
+-rw-r--r--   0        0        0     3229 2023-07-25 19:11:52.197217 dnspython-2.4.1/dns/rdtypes/ANY/HIP.py
+-rw-r--r--   0        0        0     2714 2023-07-25 19:11:52.197362 dnspython-2.4.1/dns/rdtypes/ANY/ISDN.py
+-rw-r--r--   0        0        0     1287 2023-07-25 19:11:52.197507 dnspython-2.4.1/dns/rdtypes/ANY/L32.py
+-rw-r--r--   0        0        0     1593 2023-07-25 19:11:52.197647 dnspython-2.4.1/dns/rdtypes/ANY/L64.py
+-rw-r--r--   0        0        0    12025 2023-07-25 19:11:52.197792 dnspython-2.4.1/dns/rdtypes/ANY/LOC.py
+-rw-r--r--   0        0        0     1339 2023-07-25 19:11:52.197926 dnspython-2.4.1/dns/rdtypes/ANY/LP.py
+-rw-r--r--   0        0        0      996 2023-07-25 19:11:52.198027 dnspython-2.4.1/dns/rdtypes/ANY/MX.py
+-rw-r--r--   0        0        0     1545 2023-07-25 19:11:52.198168 dnspython-2.4.1/dns/rdtypes/ANY/NID.py
+-rw-r--r--   0        0        0     1042 2023-07-25 19:11:52.198273 dnspython-2.4.1/dns/rdtypes/ANY/NINFO.py
+-rw-r--r--   0        0        0      996 2023-07-25 19:11:52.198380 dnspython-2.4.1/dns/rdtypes/ANY/NS.py
+-rw-r--r--   0        0        0     2476 2023-07-25 19:11:52.198499 dnspython-2.4.1/dns/rdtypes/ANY/NSEC.py
+-rw-r--r--   0        0        0     4152 2023-07-25 19:11:52.198617 dnspython-2.4.1/dns/rdtypes/ANY/NSEC3.py
+-rw-r--r--   0        0        0     2636 2023-07-25 19:11:52.198739 dnspython-2.4.1/dns/rdtypes/ANY/NSEC3PARAM.py
+-rw-r--r--   0        0        0     1852 2023-07-25 19:11:52.198877 dnspython-2.4.1/dns/rdtypes/ANY/OPENPGPKEY.py
+-rw-r--r--   0        0        0     2562 2023-07-25 19:11:52.198990 dnspython-2.4.1/dns/rdtypes/ANY/OPT.py
+-rw-r--r--   0        0        0      998 2023-07-25 19:11:52.199108 dnspython-2.4.1/dns/rdtypes/ANY/PTR.py
+-rw-r--r--   0        0        0     2185 2023-07-25 19:11:52.199230 dnspython-2.4.1/dns/rdtypes/ANY/RP.py
+-rw-r--r--   0        0        0     4924 2023-07-25 19:11:52.199353 dnspython-2.4.1/dns/rdtypes/ANY/RRSIG.py
+-rw-r--r--   0        0        0     1014 2023-07-25 19:11:52.199460 dnspython-2.4.1/dns/rdtypes/ANY/RT.py
+-rw-r--r--   0        0        0      222 2023-07-25 19:11:52.199515 dnspython-2.4.1/dns/rdtypes/ANY/SMIMEA.py
+-rw-r--r--   0        0        0     3146 2023-07-25 19:11:52.199647 dnspython-2.4.1/dns/rdtypes/ANY/SOA.py
+-rw-r--r--   0        0        0     1023 2023-07-25 19:11:52.199782 dnspython-2.4.1/dns/rdtypes/ANY/SPF.py
+-rw-r--r--   0        0        0     2531 2023-07-25 19:11:52.199922 dnspython-2.4.1/dns/rdtypes/ANY/SSHFP.py
+-rw-r--r--   0        0        0     4932 2023-07-25 19:11:52.200075 dnspython-2.4.1/dns/rdtypes/ANY/TKEY.py
+-rw-r--r--   0        0        0      219 2023-07-25 19:11:52.200171 dnspython-2.4.1/dns/rdtypes/ANY/TLSA.py
+-rw-r--r--   0        0        0     4751 2023-07-25 19:11:52.200351 dnspython-2.4.1/dns/rdtypes/ANY/TSIG.py
+-rw-r--r--   0        0        0     1001 2023-07-25 19:11:52.200481 dnspython-2.4.1/dns/rdtypes/ANY/TXT.py
+-rw-r--r--   0        0        0     2922 2023-07-25 19:11:52.200612 dnspython-2.4.1/dns/rdtypes/ANY/URI.py
+-rw-r--r--   0        0        0     1945 2023-07-25 19:11:52.200772 dnspython-2.4.1/dns/rdtypes/ANY/X25.py
+-rw-r--r--   0        0        0     2394 2023-07-25 19:11:52.200910 dnspython-2.4.1/dns/rdtypes/ANY/ZONEMD.py
+-rw-r--r--   0        0        0     1497 2023-07-25 19:11:52.201076 dnspython-2.4.1/dns/rdtypes/ANY/__init__.py
+-rw-r--r--   0        0        0     2217 2023-07-25 19:11:52.201259 dnspython-2.4.1/dns/rdtypes/CH/A.py
+-rw-r--r--   0        0        0      923 2023-07-25 19:11:52.201427 dnspython-2.4.1/dns/rdtypes/CH/__init__.py
+-rw-r--r--   0        0        0     1815 2023-07-25 19:11:52.201614 dnspython-2.4.1/dns/rdtypes/IN/A.py
+-rw-r--r--   0        0        0     1821 2023-07-25 19:11:52.201778 dnspython-2.4.1/dns/rdtypes/IN/AAAA.py
+-rw-r--r--   0        0        0     5099 2023-07-25 19:11:52.201911 dnspython-2.4.1/dns/rdtypes/IN/APL.py
+-rw-r--r--   0        0        0     1857 2023-07-25 19:11:52.202065 dnspython-2.4.1/dns/rdtypes/IN/DHCID.py
+-rw-r--r--   0        0        0      220 2023-07-25 19:11:52.202199 dnspython-2.4.1/dns/rdtypes/IN/HTTPS.py
+-rw-r--r--   0        0        0     3291 2023-07-25 19:11:52.202346 dnspython-2.4.1/dns/rdtypes/IN/IPSECKEY.py
+-rw-r--r--   0        0        0     1014 2023-07-25 19:11:52.202481 dnspython-2.4.1/dns/rdtypes/IN/KX.py
+-rw-r--r--   0        0        0     3751 2023-07-25 19:11:52.202644 dnspython-2.4.1/dns/rdtypes/IN/NAPTR.py
+-rw-r--r--   0        0        0     2166 2023-07-25 19:11:52.202811 dnspython-2.4.1/dns/rdtypes/IN/NSAP.py
+-rw-r--r--   0        0        0     1016 2023-07-25 19:11:52.202956 dnspython-2.4.1/dns/rdtypes/IN/NSAP_PTR.py
+-rw-r--r--   0        0        0     2757 2023-07-25 19:11:52.203091 dnspython-2.4.1/dns/rdtypes/IN/PX.py
+-rw-r--r--   0        0        0     2770 2023-07-25 19:11:52.203234 dnspython-2.4.1/dns/rdtypes/IN/SRV.py
+-rw-r--r--   0        0        0      218 2023-07-25 19:11:52.203354 dnspython-2.4.1/dns/rdtypes/IN/SVCB.py
+-rw-r--r--   0        0        0     3653 2023-07-25 19:11:52.203509 dnspython-2.4.1/dns/rdtypes/IN/WKS.py
+-rw-r--r--   0        0        0     1083 2023-07-25 19:11:52.203680 dnspython-2.4.1/dns/rdtypes/IN/__init__.py
+-rw-r--r--   0        0        0     1073 2023-07-25 19:11:52.203845 dnspython-2.4.1/dns/rdtypes/__init__.py
+-rw-r--r--   0        0        0     2857 2023-07-25 19:11:52.203993 dnspython-2.4.1/dns/rdtypes/dnskeybase.py
+-rw-r--r--   0        0        0     3428 2023-07-25 19:11:52.204122 dnspython-2.4.1/dns/rdtypes/dsbase.py
+-rw-r--r--   0        0        0     2631 2023-07-25 19:11:52.204244 dnspython-2.4.1/dns/rdtypes/euibase.py
+-rw-r--r--   0        0        0     3199 2023-07-25 19:11:52.204393 dnspython-2.4.1/dns/rdtypes/mxbase.py
+-rw-r--r--   0        0        0     2325 2023-07-25 19:11:52.204541 dnspython-2.4.1/dns/rdtypes/nsbase.py
+-rw-r--r--   0        0        0    16952 2023-07-25 19:11:52.204718 dnspython-2.4.1/dns/rdtypes/svcbbase.py
+-rw-r--r--   0        0        0     2597 2023-07-25 19:11:52.204867 dnspython-2.4.1/dns/rdtypes/tlsabase.py
+-rw-r--r--   0        0        0     3630 2023-07-25 19:11:52.204991 dnspython-2.4.1/dns/rdtypes/txtbase.py
+-rw-r--r--   0        0        0     9003 2023-07-25 19:11:52.205133 dnspython-2.4.1/dns/rdtypes/util.py
+-rw-r--r--   0        0        0    10673 2023-07-25 19:11:52.205282 dnspython-2.4.1/dns/renderer.py
+-rw-r--r--   0        0        0    73540 2023-07-25 19:11:52.205626 dnspython-2.4.1/dns/resolver.py
+-rw-r--r--   0        0        0     3828 2023-07-25 19:11:52.205761 dnspython-2.4.1/dns/reversename.py
+-rw-r--r--   0        0        0     9168 2023-07-25 19:11:52.205903 dnspython-2.4.1/dns/rrset.py
+-rw-r--r--   0        0        0     3606 2023-07-25 19:11:52.206072 dnspython-2.4.1/dns/serial.py
+-rw-r--r--   0        0        0     9089 2023-07-25 19:11:52.206223 dnspython-2.4.1/dns/set.py
+-rw-r--r--   0        0        0    23583 2023-07-25 19:11:52.206375 dnspython-2.4.1/dns/tokenizer.py
+-rw-r--r--   0        0        0    22660 2023-07-25 19:11:52.206570 dnspython-2.4.1/dns/transaction.py
+-rw-r--r--   0        0        0    11422 2023-07-25 19:11:52.206725 dnspython-2.4.1/dns/tsig.py
+-rw-r--r--   0        0        0     2633 2023-07-25 19:11:52.206863 dnspython-2.4.1/dns/tsigkeyring.py
+-rw-r--r--   0        0        0     2979 2023-07-25 19:11:52.207035 dnspython-2.4.1/dns/ttl.py
+-rw-r--r--   0        0        0    12243 2023-07-25 19:11:52.207181 dnspython-2.4.1/dns/update.py
+-rw-r--r--   0        0        0     1926 2023-07-25 19:11:59.370075 dnspython-2.4.1/dns/version.py
+-rw-r--r--   0        0        0    11765 2023-07-25 19:11:52.207450 dnspython-2.4.1/dns/versioned.py
+-rw-r--r--   0        0        0     9005 2023-07-25 19:11:52.207555 dnspython-2.4.1/dns/win32util.py
+-rw-r--r--   0        0        0     2830 2023-07-25 19:11:52.207682 dnspython-2.4.1/dns/wire.py
+-rw-r--r--   0        0        0    13273 2023-07-25 19:11:52.207836 dnspython-2.4.1/dns/xfr.py
+-rw-r--r--   0        0        0    51093 2023-07-25 19:11:52.208090 dnspython-2.4.1/dns/zone.py
+-rw-r--r--   0        0        0    27930 2023-07-25 19:11:52.208302 dnspython-2.4.1/dns/zonefile.py
+-rw-r--r--   0        0        0      690 2023-07-25 19:11:52.208433 dnspython-2.4.1/dns/zonetypes.py
+-rw-r--r--   0        0        0      874 2023-07-25 19:11:52.213953 dnspython-2.4.1/examples/async_dns.py
+-rwxr-xr-x   0        0        0     1194 2023-07-25 19:11:52.214064 dnspython-2.4.1/examples/ddns.py
+-rw-r--r--   0        0        0      950 2023-07-25 19:11:52.214144 dnspython-2.4.1/examples/ddr.py
+-rwxr-xr-x   0        0        0     3001 2023-07-25 19:11:52.214237 dnspython-2.4.1/examples/doh-json.py
+-rwxr-xr-x   0        0        0      534 2023-07-25 19:11:52.214314 dnspython-2.4.1/examples/doh.py
+-rw-r--r--   0        0        0     3143 2023-07-25 19:11:52.214490 dnspython-2.4.1/examples/doq.py
+-rwxr-xr-x   0        0        0      115 2023-07-25 19:11:52.214579 dnspython-2.4.1/examples/e164.py
+-rwxr-xr-x   0        0        0      450 2023-07-25 19:11:52.214662 dnspython-2.4.1/examples/ecs.py
+-rwxr-xr-x   0        0        0     1739 2023-07-25 19:11:52.214747 dnspython-2.4.1/examples/edns.py
+-rw-r--r--   0        0        0     1532 2023-07-25 19:11:52.214830 dnspython-2.4.1/examples/edns_resolver.py
+-rwxr-xr-x   0        0        0      189 2023-07-25 19:11:52.214938 dnspython-2.4.1/examples/mx.py
+-rwxr-xr-x   0        0        0      356 2023-07-25 19:11:52.215046 dnspython-2.4.1/examples/name.py
+-rw-r--r--   0        0        0     1655 2023-07-25 19:11:52.215135 dnspython-2.4.1/examples/query_specific.py
+-rw-r--r--   0        0        0     1022 2023-07-25 19:11:52.215241 dnspython-2.4.1/examples/receive_notify.py
+-rwxr-xr-x   0        0        0     1389 2023-07-25 19:11:52.215328 dnspython-2.4.1/examples/reverse.py
+-rwxr-xr-x   0        0        0      140 2023-07-25 19:11:52.215419 dnspython-2.4.1/examples/reverse_name.py
+-rwxr-xr-x   0        0        0      340 2023-07-25 19:11:52.215523 dnspython-2.4.1/examples/xfr.py
+-rwxr-xr-x   0        0        0    12173 2023-07-25 19:11:52.215657 dnspython-2.4.1/examples/zonediff.py
+-rw-r--r--   0        0        0     2180 2023-07-25 19:11:59.370869 dnspython-2.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1967 2023-07-25 19:11:59.371031 dnspython-2.4.1/setup.cfg
+-rw-r--r--   0        0        0        0 2023-07-25 19:11:52.216292 dnspython-2.4.1/tests/__init__.py
+-rw-r--r--   0        0        0    12881 2023-07-25 19:11:52.216428 dnspython-2.4.1/tests/example
+-rw-r--r--   0        0        0    11010 2023-07-25 19:11:52.216543 dnspython-2.4.1/tests/example1.good
+-rw-r--r--   0        0        0    12699 2023-07-25 19:11:52.216658 dnspython-2.4.1/tests/example2.good
+-rw-r--r--   0        0        0    11010 2023-07-25 19:11:52.216768 dnspython-2.4.1/tests/example3.good
+-rw-r--r--   0        0        0    11027 2023-07-25 19:11:52.216875 dnspython-2.4.1/tests/example4.good
+-rw-r--r--   0        0        0     8696 2023-07-25 19:11:52.217102 dnspython-2.4.1/tests/keys.py
+-rw-r--r--   0        0        0       91 2023-07-25 19:11:52.217225 dnspython-2.4.1/tests/md_module.py
+-rw-r--r--   0        0        0      223 2023-07-25 19:11:52.217316 dnspython-2.4.1/tests/mx-2-0.pickle
+-rw-r--r--   0        0        0    11832 2023-07-25 19:11:52.217574 dnspython-2.4.1/tests/nanonameserver.py
+-rw-r--r--   0        0        0     4416 2023-07-25 19:11:52.217704 dnspython-2.4.1/tests/nanoquic.py
+-rw-r--r--   0        0        0      140 2023-07-25 19:11:52.217763 dnspython-2.4.1/tests/query
+-rw-r--r--   0        0        0      111 2023-07-25 19:11:52.217929 dnspython-2.4.1/tests/stxt_module.py
+-rw-r--r--   0        0        0     4573 2023-07-25 19:11:52.218013 dnspython-2.4.1/tests/svcb_test_vectors.generic
+-rw-r--r--   0        0        0     1157 2023-07-25 19:11:52.218070 dnspython-2.4.1/tests/svcb_test_vectors.text
+-rw-r--r--   0        0        0    21140 2023-07-25 19:11:52.218229 dnspython-2.4.1/tests/test_address.py
+-rw-r--r--   0        0        0    24243 2023-07-25 19:11:52.218397 dnspython-2.4.1/tests/test_async.py
+-rw-r--r--   0        0        0     3752 2023-07-25 19:11:52.218544 dnspython-2.4.1/tests/test_bugs.py
+-rw-r--r--   0        0        0     1295 2023-07-25 19:11:52.218663 dnspython-2.4.1/tests/test_constants.py
+-rw-r--r--   0        0        0     1258 2023-07-25 19:11:52.218773 dnspython-2.4.1/tests/test_ddr.py
+-rw-r--r--   0        0        0    51304 2023-07-25 19:11:52.219018 dnspython-2.4.1/tests/test_dnssec.py
+-rw-r--r--   0        0        0    10264 2023-07-25 19:11:52.219152 dnspython-2.4.1/tests/test_dnssecalgs.py
+-rw-r--r--   0        0        0     7192 2023-07-25 19:11:52.219267 dnspython-2.4.1/tests/test_doh.py
+-rw-r--r--   0        0        0     1800 2023-07-25 19:11:52.219371 dnspython-2.4.1/tests/test_doq.py
+-rw-r--r--   0        0        0     8926 2023-07-25 19:11:52.219497 dnspython-2.4.1/tests/test_edns.py
+-rw-r--r--   0        0        0     1977 2023-07-25 19:11:52.219620 dnspython-2.4.1/tests/test_entropy.py
+-rw-r--r--   0        0        0     2192 2023-07-25 19:11:52.219800 dnspython-2.4.1/tests/test_exceptions.py
+-rw-r--r--   0        0        0     2914 2023-07-25 19:11:52.220008 dnspython-2.4.1/tests/test_flags.py
+-rw-r--r--   0        0        0    24372 2023-07-25 19:11:52.220170 dnspython-2.4.1/tests/test_generate.py
+-rw-r--r--   0        0        0     3055 2023-07-25 19:11:52.220303 dnspython-2.4.1/tests/test_grange.py
+-rw-r--r--   0        0        0     4384 2023-07-25 19:11:52.220419 dnspython-2.4.1/tests/test_immutable.py
+-rw-r--r--   0        0        0    27696 2023-07-25 19:11:52.220576 dnspython-2.4.1/tests/test_message.py
+-rw-r--r--   0        0        0    37873 2023-07-25 19:11:52.220859 dnspython-2.4.1/tests/test_name.py
+-rw-r--r--   0        0        0     5625 2023-07-25 19:11:52.221007 dnspython-2.4.1/tests/test_namedict.py
+-rw-r--r--   0        0        0     1907 2023-07-25 19:11:52.221123 dnspython-2.4.1/tests/test_nsec3.py
+-rw-r--r--   0        0        0     3685 2023-07-25 19:11:52.221228 dnspython-2.4.1/tests/test_nsec3_hash.py
+-rw-r--r--   0        0        0    10872 2023-07-25 19:11:52.221341 dnspython-2.4.1/tests/test_ntoaaton.py
+-rw-r--r--   0        0        0     4037 2023-07-25 19:11:52.221487 dnspython-2.4.1/tests/test_processing_order.py
+-rw-r--r--   0        0        0    24274 2023-07-25 19:11:52.221634 dnspython-2.4.1/tests/test_query.py
+-rw-r--r--   0        0        0    43483 2023-07-25 19:11:52.221841 dnspython-2.4.1/tests/test_rdata.py
+-rw-r--r--   0        0        0     6136 2023-07-25 19:11:52.221987 dnspython-2.4.1/tests/test_rdataset.py
+-rw-r--r--   0        0        0     4307 2023-07-25 19:11:52.222088 dnspython-2.4.1/tests/test_rdtypeandclass.py
+-rw-r--r--   0        0        0     1696 2023-07-25 19:11:52.222208 dnspython-2.4.1/tests/test_rdtypeanydnskey.py
+-rw-r--r--   0        0        0     7283 2023-07-25 19:11:52.222329 dnspython-2.4.1/tests/test_rdtypeanyeui.py
+-rw-r--r--   0        0        0     3437 2023-07-25 19:11:52.222452 dnspython-2.4.1/tests/test_rdtypeanyloc.py
+-rw-r--r--   0        0        0     4309 2023-07-25 19:11:52.222562 dnspython-2.4.1/tests/test_rdtypeanytkey.py
+-rw-r--r--   0        0        0     3972 2023-07-25 19:11:52.222772 dnspython-2.4.1/tests/test_renderer.py
+-rw-r--r--   0        0        0    21664 2023-07-25 19:11:52.222904 dnspython-2.4.1/tests/test_resolution.py
+-rw-r--r--   0        0        0    45216 2023-07-25 19:11:52.223105 dnspython-2.4.1/tests/test_resolver.py
+-rw-r--r--   0        0        0     8942 2023-07-25 19:11:52.223314 dnspython-2.4.1/tests/test_resolver_override.py
+-rw-r--r--   0        0        0     8220 2023-07-25 19:11:52.223450 dnspython-2.4.1/tests/test_rrset.py
+-rw-r--r--   0        0        0     3920 2023-07-25 19:11:52.223571 dnspython-2.4.1/tests/test_rrset_reader.py
+-rw-r--r--   0        0        0     3776 2023-07-25 19:11:52.223693 dnspython-2.4.1/tests/test_serial.py
+-rw-r--r--   0        0        0     8872 2023-07-25 19:11:52.223816 dnspython-2.4.1/tests/test_set.py
+-rw-r--r--   0        0        0    14173 2023-07-25 19:11:52.223954 dnspython-2.4.1/tests/test_svcb.py
+-rw-r--r--   0        0        0    13465 2023-07-25 19:11:52.224087 dnspython-2.4.1/tests/test_tokenizer.py
+-rw-r--r--   0        0        0    22137 2023-07-25 19:11:52.224229 dnspython-2.4.1/tests/test_transaction.py
+-rw-r--r--   0        0        0    12773 2023-07-25 19:11:52.224438 dnspython-2.4.1/tests/test_tsig.py
+-rw-r--r--   0        0        0     2072 2023-07-25 19:11:52.224557 dnspython-2.4.1/tests/test_tsigkeyring.py
+-rw-r--r--   0        0        0     1120 2023-07-25 19:11:52.224663 dnspython-2.4.1/tests/test_ttl.py
+-rw-r--r--   0        0        0    11423 2023-07-25 19:11:52.224789 dnspython-2.4.1/tests/test_update.py
+-rw-r--r--   0        0        0     3308 2023-07-25 19:11:52.224903 dnspython-2.4.1/tests/test_wire.py
+-rw-r--r--   0        0        0    21524 2023-07-25 19:11:52.225020 dnspython-2.4.1/tests/test_xfr.py
+-rw-r--r--   0        0        0    45309 2023-07-25 19:11:52.225216 dnspython-2.4.1/tests/test_zone.py
+-rw-r--r--   0        0        0     9119 2023-07-25 19:11:52.225352 dnspython-2.4.1/tests/test_zonedigest.py
+-rw-r--r--   0        0        0     1204 2023-07-25 19:11:52.225574 dnspython-2.4.1/tests/tls/ca.crt
+-rw-r--r--   0        0        0      119 2023-07-25 19:11:52.225777 dnspython-2.4.1/tests/tls/private.pem
+-rw-r--r--   0        0        0     2095 2023-07-25 19:11:52.225890 dnspython-2.4.1/tests/tls/public.crt
+-rw-r--r--   0        0        0      101 2023-07-25 19:11:52.225989 dnspython-2.4.1/tests/ttxt_module.py
+-rw-r--r--   0        0        0      372 2023-07-25 19:11:52.226095 dnspython-2.4.1/tests/utest.py
+-rw-r--r--   0        0        0     4215 2023-07-25 19:11:52.226275 dnspython-2.4.1/tests/util.py
+-rwxr-xr-x   0        0        0     3126 2023-07-25 19:11:52.226368 dnspython-2.4.1/util/constants-tool
+-rw-r--r--   0        0        0      437 2023-07-25 19:11:52.226490 dnspython-2.4.1/util/generate-mx-pickle.py
+-rw-r--r--   0        0        0      358 2023-07-25 19:11:52.226696 dnspython-2.4.1/util/generate-rdatatype-doc.py
+-rw-r--r--   0        0        0     4892 1970-01-01 00:00:00.000000 dnspython-2.4.1/PKG-INFO
```

### Comparing `dnspython-2.4.0rc1/LICENSE` & `dnspython-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/README.md` & `dnspython-2.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -26,33 +26,35 @@
 `socket.gethostbyname()`.
 
 dnspython originated at Nominum where it was developed
 to facilitate the testing of DNS software.
 
 ## ABOUT THIS RELEASE
 
-This is dnspython 2.4.0rc1.
+This is dnspython 2.4.1.
 Please read
-[What's New](https://dnspython.readthedocs.io/en/latest/whatsnew.html) for
+[What's New](https://dnspython.readthedocs.io/en/stable/whatsnew.html) for
 information about the changes in this release.
 
 ## INSTALLATION
 
 * Many distributions have dnspython packaged for you, so you should
   check there first.
 * To use a wheel downloaded from PyPi, run:
 
     pip install dnspython
 
 * To install from the source code, go into the top-level of the source code
   and run:
 
+```
     pip install --upgrade pip build
     python -m build
     pip install dist/*.whl
+```
 
 * To install the latest from the master branch, run `pip install git+https://github.com/rthalley/dnspython.git`
 
 Dnspython's default installation does not depend on any modules other than
 those in the Python standard library.  To use some features, additional modules
 must be installed.  For convenience, pip options are defined for the
 requirements.
```

### Comparing `dnspython-2.4.0rc1/dns/__init__.py` & `dnspython-2.4.1/dns/__init__.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/_asyncbackend.py` & `dnspython-2.4.1/dns/_asyncbackend.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/_asyncio_backend.py` & `dnspython-2.4.1/dns/_asyncio_backend.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,22 @@
 
     def error_received(self, exc):  # pragma: no cover
         if self.recvfrom and not self.recvfrom.done():
             self.recvfrom.set_exception(exc)
 
     def connection_lost(self, exc):
         if self.recvfrom and not self.recvfrom.done():
-            self.recvfrom.set_exception(exc)
+            if exc is None:
+                # EOF we triggered.  Is there a better way to do this?
+                try:
+                    raise EOFError
+                except EOFError as e:
+                    self.recvfrom.set_exception(e)
+            else:
+                self.recvfrom.set_exception(exc)
 
     def close(self):
         self.transport.close()
 
 
 async def _maybe_wait_for(awaitable, timeout):
     if timeout:
@@ -99,39 +106,37 @@
         return await _maybe_wait_for(self.writer.drain(), timeout)
 
     async def recv(self, size, timeout):
         return await _maybe_wait_for(self.reader.read(size), timeout)
 
     async def close(self):
         self.writer.close()
-        try:
-            await self.writer.wait_closed()
-        except AttributeError:  # pragma: no cover
-            pass
 
     async def getpeername(self):
         return self.writer.get_extra_info("peername")
 
     async def getsockname(self):
         return self.writer.get_extra_info("sockname")
 
     async def getpeercert(self, timeout):
         return self.writer.get_extra_info("peercert")
 
 
 try:
     import anyio
     import httpcore
-    import httpcore.backends.asyncio
-    import httpcore.backends.base
+    import httpcore._backends.anyio
     import httpx
 
+    _CoreAsyncNetworkBackend = httpcore.AsyncNetworkBackend
+    _CoreAnyIOStream = httpcore._backends.anyio.AnyIOStream
+
     from dns.query import _compute_times, _expiration_for_this_attempt, _remaining
 
-    class _NetworkBackend(httpcore.backends.base.AsyncNetworkBackend):
+    class _NetworkBackend(_CoreAsyncNetworkBackend):
         def __init__(self, resolver, local_port, bootstrap_address, family):
             super().__init__()
             self._local_port = local_port
             self._resolver = resolver
             self._bootstrap_address = bootstrap_address
             self._family = family
             if local_port != 0:
@@ -163,15 +168,15 @@
                     timeout = _remaining(attempt_expiration)
                     with anyio.fail_after(timeout):
                         stream = await anyio.connect_tcp(
                             remote_host=address,
                             remote_port=port,
                             local_host=local_address,
                         )
-                    return httpcore.backends.asyncio.AsyncIOStream(stream)
+                    return _CoreAnyIOStream(stream)
                 except Exception:
                     pass
             raise httpcore.ConnectError
 
         async def connect_unix_socket(
             self, path, timeout, socket_options=None
         ):  # pylint: disable=signature-differs
```

### Comparing `dnspython-2.4.0rc1/dns/_ddr.py` & `dnspython-2.4.1/dns/_ddr.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/_immutable_ctx.py` & `dnspython-2.4.1/dns/_immutable_ctx.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/_trio_backend.py` & `dnspython-2.4.1/dns/_trio_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,21 +93,23 @@
             return self.stream.getpeercert()
         else:
             raise NotImplementedError
 
 
 try:
     import httpcore
-    import httpcore.backends.base
-    import httpcore.backends.trio
+    import httpcore._backends.trio
     import httpx
 
+    _CoreAsyncNetworkBackend = httpcore.AsyncNetworkBackend
+    _CoreTrioStream = httpcore._backends.trio.TrioStream
+
     from dns.query import _compute_times, _expiration_for_this_attempt, _remaining
 
-    class _NetworkBackend(httpcore.backends.base.AsyncNetworkBackend):
+    class _NetworkBackend(_CoreAsyncNetworkBackend):
         def __init__(self, resolver, local_port, bootstrap_address, family):
             super().__init__()
             self._local_port = local_port
             self._resolver = resolver
             self._bootstrap_address = bootstrap_address
             self._family = family
 
@@ -138,15 +140,15 @@
                         source = None
                     destination = (address, port)
                     attempt_expiration = _expiration_for_this_attempt(2.0, expiration)
                     timeout = _remaining(attempt_expiration)
                     sock = await Backend().make_socket(
                         af, socket.SOCK_STREAM, 0, source, destination, timeout
                     )
-                    return httpcore.backends.trio.TrioStream(sock.stream)
+                    return _CoreTrioStream(sock.stream)
                 except Exception:
                     continue
             raise httpcore.ConnectError
 
         async def connect_unix_socket(
             self, path, timeout, socket_options=None
         ):  # pylint: disable=signature-differs
```

### Comparing `dnspython-2.4.0rc1/dns/asyncbackend.py` & `dnspython-2.4.1/dns/asyncbackend.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/asyncquery.py` & `dnspython-2.4.1/dns/asyncquery.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     BadResponse,
     NoDOH,
     NoDOQ,
     UDPMode,
     _compute_times,
     _have_http2,
     _matches_destination,
+    _remaining,
     have_doh,
     ssl,
 )
 
 if have_doh:
     import httpx
 
@@ -439,17 +440,14 @@
     else:
         if ssl_context is None:
             # See the comment about ssl.create_default_context() in query.py
             ssl_context = ssl.create_default_context()  # lgtm[py/insecure-protocol]
             ssl_context.minimum_version = ssl.TLSVersion.TLSv1_2
             if server_hostname is None:
                 ssl_context.check_hostname = False
-        else:
-            ssl_context = None
-            server_hostname = None
         af = dns.inet.af_for_address(where)
         stuple = _source_tuple(af, source, source_port)
         dtuple = (where, port)
         if not backend:
             backend = dns.asyncbackend.get_default_backend()
         cm = await backend.make_socket(
             af,
@@ -735,19 +733,19 @@
 
     async with cfactory() as context:
         async with mfactory(
             context, verify_mode=verify, server_name=server_hostname
         ) as the_manager:
             if not connection:
                 the_connection = the_manager.connect(where, port, source, source_port)
-            start = time.time()
-            stream = await the_connection.make_stream()
+            (start, expiration) = _compute_times(timeout)
+            stream = await the_connection.make_stream(timeout)
             async with stream:
                 await stream.send(wire, True)
-                wire = await stream.receive(timeout)
+                wire = await stream.receive(_remaining(expiration))
             finish = time.time()
         r = dns.message.from_wire(
             wire,
             keyring=q.keyring,
             request_mac=q.request_mac,
             one_rr_per_rrset=one_rr_per_rrset,
             ignore_trailing=ignore_trailing,
```

### Comparing `dnspython-2.4.0rc1/dns/asyncresolver.py` & `dnspython-2.4.1/dns/asyncresolver.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/dnssec.py` & `dnspython-2.4.1/dns/dnssec.py`

 * *Files 1% similar despite different names*

```diff
@@ -301,15 +301,18 @@
     else:
         rdataset = value
     if rdataset is None:
         return None
     return [
         cast(DNSKEY, rd)
         for rd in rdataset
-        if rd.algorithm == rrsig.algorithm and key_id(rd) == rrsig.key_tag
+        if rd.algorithm == rrsig.algorithm
+        and key_id(rd) == rrsig.key_tag
+        and (rd.flags & Flag.ZONE) == Flag.ZONE  # RFC 4034 2.1.1
+        and rd.protocol == 3  # RFC 4034 2.1.2
     ]
 
 
 def _get_rrname_rdataset(
     rrset: Union[dns.rrset.RRset, Tuple[dns.name.Name, dns.rdataset.Rdataset]],
 ) -> Tuple[dns.name.Name, dns.rdataset.Rdataset]:
     if isinstance(rrset, tuple):
```

### Comparing `dnspython-2.4.0rc1/dns/dnssecalgs/__init__.py` & `dnspython-2.4.1/dns/dnssecalgs/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,51 @@
 from typing import Dict, Optional, Tuple, Type, Union
 
 import dns.name
-from dns.dnssecalgs.base import GenericPrivateKey
-from dns.dnssecalgs.dsa import PrivateDSA, PrivateDSANSEC3SHA1
-from dns.dnssecalgs.ecdsa import PrivateECDSAP256SHA256, PrivateECDSAP384SHA384
-from dns.dnssecalgs.eddsa import PrivateED448, PrivateED25519
-from dns.dnssecalgs.rsa import (
-    PrivateRSAMD5,
-    PrivateRSASHA1,
-    PrivateRSASHA1NSEC3SHA1,
-    PrivateRSASHA256,
-    PrivateRSASHA512,
-)
+
+try:
+    from dns.dnssecalgs.base import GenericPrivateKey
+    from dns.dnssecalgs.dsa import PrivateDSA, PrivateDSANSEC3SHA1
+    from dns.dnssecalgs.ecdsa import PrivateECDSAP256SHA256, PrivateECDSAP384SHA384
+    from dns.dnssecalgs.eddsa import PrivateED448, PrivateED25519
+    from dns.dnssecalgs.rsa import (
+        PrivateRSAMD5,
+        PrivateRSASHA1,
+        PrivateRSASHA1NSEC3SHA1,
+        PrivateRSASHA256,
+        PrivateRSASHA512,
+    )
+
+    _have_cryptography = True
+except ImportError:
+    _have_cryptography = False
+
 from dns.dnssectypes import Algorithm
 from dns.exception import UnsupportedAlgorithm
 from dns.rdtypes.ANY.DNSKEY import DNSKEY
 
 AlgorithmPrefix = Optional[Union[bytes, dns.name.Name]]
 
-algorithms: Dict[Tuple[Algorithm, AlgorithmPrefix], Type[GenericPrivateKey]] = {
-    (Algorithm.RSAMD5, None): PrivateRSAMD5,
-    (Algorithm.DSA, None): PrivateDSA,
-    (Algorithm.RSASHA1, None): PrivateRSASHA1,
-    (Algorithm.DSANSEC3SHA1, None): PrivateDSANSEC3SHA1,
-    (Algorithm.RSASHA1NSEC3SHA1, None): PrivateRSASHA1NSEC3SHA1,
-    (Algorithm.RSASHA256, None): PrivateRSASHA256,
-    (Algorithm.RSASHA512, None): PrivateRSASHA512,
-    (Algorithm.ECDSAP256SHA256, None): PrivateECDSAP256SHA256,
-    (Algorithm.ECDSAP384SHA384, None): PrivateECDSAP384SHA384,
-    (Algorithm.ED25519, None): PrivateED25519,
-    (Algorithm.ED448, None): PrivateED448,
-}
+algorithms: Dict[Tuple[Algorithm, AlgorithmPrefix], Type[GenericPrivateKey]] = {}
+if _have_cryptography:
+    algorithms.update(
+        {
+            (Algorithm.RSAMD5, None): PrivateRSAMD5,
+            (Algorithm.DSA, None): PrivateDSA,
+            (Algorithm.RSASHA1, None): PrivateRSASHA1,
+            (Algorithm.DSANSEC3SHA1, None): PrivateDSANSEC3SHA1,
+            (Algorithm.RSASHA1NSEC3SHA1, None): PrivateRSASHA1NSEC3SHA1,
+            (Algorithm.RSASHA256, None): PrivateRSASHA256,
+            (Algorithm.RSASHA512, None): PrivateRSASHA512,
+            (Algorithm.ECDSAP256SHA256, None): PrivateECDSAP256SHA256,
+            (Algorithm.ECDSAP384SHA384, None): PrivateECDSAP384SHA384,
+            (Algorithm.ED25519, None): PrivateED25519,
+            (Algorithm.ED448, None): PrivateED448,
+        }
+    )
 
 
 def get_algorithm_cls(
     algorithm: Union[int, str], prefix: AlgorithmPrefix = None
 ) -> Type[GenericPrivateKey]:
     """Get Private Key class from Algorithm.
```

### Comparing `dnspython-2.4.0rc1/dns/dnssecalgs/base.py` & `dnspython-2.4.1/dns/dnssecalgs/base.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/dnssecalgs/cryptography.py` & `dnspython-2.4.1/dns/dnssecalgs/cryptography.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/dnssecalgs/dsa.py` & `dnspython-2.4.1/dns/dnssecalgs/dsa.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/dnssecalgs/ecdsa.py` & `dnspython-2.4.1/dns/dnssecalgs/ecdsa.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/dnssecalgs/eddsa.py` & `dnspython-2.4.1/dns/dnssecalgs/eddsa.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/dnssecalgs/rsa.py` & `dnspython-2.4.1/dns/dnssecalgs/rsa.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/dnssectypes.py` & `dnspython-2.4.1/dns/dnssectypes.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/e164.py` & `dnspython-2.4.1/dns/e164.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/edns.py` & `dnspython-2.4.1/dns/edns.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/entropy.py` & `dnspython-2.4.1/dns/entropy.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/enum.py` & `dnspython-2.4.1/dns/enum.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/exception.py` & `dnspython-2.4.1/dns/exception.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/flags.py` & `dnspython-2.4.1/dns/flags.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/grange.py` & `dnspython-2.4.1/dns/grange.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/immutable.py` & `dnspython-2.4.1/dns/immutable.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/inet.py` & `dnspython-2.4.1/dns/inet.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/ipv4.py` & `dnspython-2.4.1/dns/ipv4.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/ipv6.py` & `dnspython-2.4.1/dns/ipv6.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/message.py` & `dnspython-2.4.1/dns/message.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/name.py` & `dnspython-2.4.1/dns/name.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/namedict.py` & `dnspython-2.4.1/dns/namedict.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/nameserver.py` & `dnspython-2.4.1/dns/nameserver.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/node.py` & `dnspython-2.4.1/dns/node.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/opcode.py` & `dnspython-2.4.1/dns/opcode.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/query.py` & `dnspython-2.4.1/dns/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,29 +56,30 @@
         return None
     return min(time.time() + timeout, expiration)
 
 
 _have_httpx = False
 _have_http2 = False
 try:
+    import httpcore
+    import httpcore._backends.sync
     import httpx
 
+    _CoreNetworkBackend = httpcore.NetworkBackend
+    _CoreSyncStream = httpcore._backends.sync.SyncStream
+
     _have_httpx = True
     try:
         # See if http2 support is available.
         with httpx.Client(http2=True):
             _have_http2 = True
     except Exception:
         pass
 
-    import httpcore
-    import httpcore.backends.base
-    import httpcore.backends.sync
-
-    class _NetworkBackend(httpcore.backends.base.NetworkBackend):
+    class _NetworkBackend(_CoreNetworkBackend):
         def __init__(self, resolver, local_port, bootstrap_address, family):
             super().__init__()
             self._local_port = local_port
             self._resolver = resolver
             self._bootstrap_address = bootstrap_address
             self._family = family
 
@@ -112,15 +113,15 @@
                 attempt_expiration = _expiration_for_this_attempt(2.0, expiration)
                 try:
                     _connect(
                         sock,
                         dns.inet.low_level_address_tuple((address, port), af),
                         attempt_expiration,
                     )
-                    return httpcore.backends.sync.SyncStream(sock)
+                    return _CoreSyncStream(sock)
                 except Exception:
                     pass
             raise httpcore.ConnectError
 
         def connect_unix_socket(
             self, path, timeout, socket_options=None
         ):  # pylint: disable=signature-differs
@@ -170,15 +171,15 @@
             pass
 
         class SSLSocket:
             pass
 
         @classmethod
         def create_default_context(cls, *args, **kwargs):
-            raise Exception("no ssl support")
+            raise Exception("no ssl support")  # pylint: disable=broad-exception-raised
 
 
 # Function used to create a socket.  Can be overridden if needed in special
 # situations.
 socket_factory = socket.socket
 
 
@@ -1180,18 +1181,18 @@
             verify_mode=verify, server_name=server_hostname
         )
         the_manager = manager  # for type checking happiness
 
     with manager:
         if not connection:
             the_connection = the_manager.connect(where, port, source, source_port)
-        start = time.time()
-        with the_connection.make_stream() as stream:
+        (start, expiration) = _compute_times(timeout)
+        with the_connection.make_stream(timeout) as stream:
             stream.send(wire, True)
-            wire = stream.receive(timeout)
+            wire = stream.receive(_remaining(expiration))
         finish = time.time()
     r = dns.message.from_wire(
         wire,
         keyring=q.keyring,
         request_mac=q.request_mac,
         one_rr_per_rrset=one_rr_per_rrset,
         ignore_trailing=ignore_trailing,
```

### Comparing `dnspython-2.4.0rc1/dns/quic/__init__.py` & `dnspython-2.4.1/dns/quic/__init__.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/quic/_asyncio.py` & `dnspython-2.4.1/dns/quic/_asyncio.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import time
 
 import aioquic.quic.configuration  # type: ignore
 import aioquic.quic.connection  # type: ignore
 import aioquic.quic.events  # type: ignore
 
 import dns.asyncbackend
+import dns.exception
 import dns.inet
 from dns.quic._common import (
     QUIC_MAX_DATAGRAM,
     AsyncQuicConnection,
     AsyncQuicManager,
     BaseQuicStream,
     UnexpectedEOF,
@@ -34,16 +35,16 @@
         while True:
             timeout = self._timeout_from_expiration(expiration)
             if self._buffer.have(amount):
                 return
             self._expecting = amount
             try:
                 await asyncio.wait_for(self._wait_for_wake_up(), timeout)
-            except Exception:
-                pass
+            except TimeoutError:
+                raise dns.exception.Timeout
             self._expecting = 0
 
     async def receive(self, timeout=None):
         expiration = self._expiration_from_timeout(timeout)
         await self.wait_for(2, expiration)
         (size,) = struct.unpack("!H", self._buffer.get(2))
         await self.wait_for(size, expiration)
@@ -83,16 +84,18 @@
         self._receiver_task = None
         self._sender_task = None
 
     async def _receiver(self):
         try:
             af = dns.inet.af_for_address(self._address)
             backend = dns.asyncbackend.get_backend("asyncio")
+            # Note that peer is a low-level address tuple, but make_socket() wants
+            # a high-level address tuple, so we convert.
             self._socket = await backend.make_socket(
-                af, socket.SOCK_DGRAM, 0, self._source, self._peer
+                af, socket.SOCK_DGRAM, 0, self._source, (self._peer[0], self._peer[1])
             )
             self._socket_created.set()
             async with self._socket:
                 while not self._done:
                     (datagram, address) = await self._socket.recvfrom(
                         QUIC_MAX_DATAGRAM, None
                     )
@@ -162,28 +165,34 @@
 
     def run(self):
         if self._closed:
             return
         self._receiver_task = asyncio.Task(self._receiver())
         self._sender_task = asyncio.Task(self._sender())
 
-    async def make_stream(self):
-        await self._handshake_complete.wait()
+    async def make_stream(self, timeout=None):
+        try:
+            await asyncio.wait_for(self._handshake_complete.wait(), timeout)
+        except TimeoutError:
+            raise dns.exception.Timeout
         if self._done:
             raise UnexpectedEOF
         stream_id = self._connection.get_next_available_stream_id(False)
         stream = AsyncioQuicStream(self, stream_id)
         self._streams[stream_id] = stream
         return stream
 
     async def close(self):
         if not self._closed:
             self._manager.closed(self._peer[0], self._peer[1])
             self._closed = True
             self._connection.close()
+            # sender might be blocked on this, so set it
+            self._socket_created.set()
+            await self._socket.close()
             async with self._wake_timer:
                 self._wake_timer.notify_all()
             try:
                 await self._receiver_task
             except asyncio.CancelledError:
                 pass
             try:
```

### Comparing `dnspython-2.4.0rc1/dns/quic/_common.py` & `dnspython-2.4.1/dns/quic/_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright (C) Dnspython Contributors, see LICENSE for text of ISC license
 
 import socket
 import struct
 import time
-from typing import Any
+from typing import Any, Optional
 
 import aioquic.quic.configuration  # type: ignore
 import aioquic.quic.connection  # type: ignore
 
 import dns.inet
 
 QUIC_MAX_DATAGRAM = 2048
@@ -130,15 +130,15 @@
     def _handle_timer(self, expiration):
         now = time.time()
         if expiration <= now:
             self._connection.handle_timer(now)
 
 
 class AsyncQuicConnection(BaseQuicConnection):
-    async def make_stream(self) -> Any:
+    async def make_stream(self, timeout: Optional[float] = None) -> Any:
         pass
 
 
 class BaseQuicManager:
     def __init__(self, conf, verify_mode, connection_factory, server_name=None):
         self._connections = {}
         self._connection_factory = connection_factory
```

### Comparing `dnspython-2.4.0rc1/dns/quic/_sync.py` & `dnspython-2.4.1/dns/quic/_sync.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import threading
 import time
 
 import aioquic.quic.configuration  # type: ignore
 import aioquic.quic.connection  # type: ignore
 import aioquic.quic.events  # type: ignore
 
+import dns.exception
 import dns.inet
 from dns.quic._common import (
     QUIC_MAX_DATAGRAM,
     BaseQuicConnection,
     BaseQuicManager,
     BaseQuicStream,
     UnexpectedEOF,
@@ -38,15 +39,15 @@
             timeout = self._timeout_from_expiration(expiration)
             with self._lock:
                 if self._buffer.have(amount):
                     return
                 self._expecting = amount
             with self._wake_up:
                 if not self._wake_up.wait(timeout):
-                    raise TimeoutError
+                    raise dns.exception.Timeout
             self._expecting = 0
 
     def receive(self, timeout=None):
         expiration = self._expiration_from_timeout(timeout)
         self.wait_for(2, expiration)
         with self._lock:
             (size,) = struct.unpack("!H", self._buffer.get(2))
@@ -167,16 +168,17 @@
 
     def run(self):
         if self._closed:
             return
         self._worker_thread = threading.Thread(target=self._worker)
         self._worker_thread.start()
 
-    def make_stream(self):
-        self._handshake_complete.wait()
+    def make_stream(self, timeout=None):
+        if not self._handshake_complete.wait(timeout):
+            raise dns.exception.Timeout
         with self._lock:
             if self._done:
                 raise UnexpectedEOF
             stream_id = self._connection.get_next_available_stream_id(False)
             stream = SyncQuicStream(self, stream_id)
             self._streams[stream_id] = stream
         return stream
```

### Comparing `dnspython-2.4.0rc1/dns/quic/_trio.py` & `dnspython-2.4.1/dns/quic/_trio.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import time
 
 import aioquic.quic.configuration  # type: ignore
 import aioquic.quic.connection  # type: ignore
 import aioquic.quic.events  # type: ignore
 import trio
 
+import dns.exception
 import dns.inet
 from dns._asyncbackend import NullContext
 from dns.quic._common import (
     QUIC_MAX_DATAGRAM,
     AsyncQuicConnection,
     AsyncQuicManager,
     BaseQuicStream,
@@ -41,14 +42,15 @@
         else:
             context = trio.move_on_after(timeout)
         with context:
             await self.wait_for(2)
             (size,) = struct.unpack("!H", self._buffer.get(2))
             await self.wait_for(size)
             return self._buffer.get(size)
+        raise dns.exception.Timeout
 
     async def send(self, datagram, is_end=False):
         data = self._encapsulate(datagram)
         await self._connection.write(self._stream_id, data, is_end)
 
     async def _add_input(self, data, is_end):
         if self._common_add_input(data, is_end):
@@ -133,22 +135,28 @@
     async def run(self):
         if self._closed:
             return
         async with trio.open_nursery() as nursery:
             nursery.start_soon(self._worker)
         self._run_done.set()
 
-    async def make_stream(self):
-        await self._handshake_complete.wait()
-        if self._done:
-            raise UnexpectedEOF
-        stream_id = self._connection.get_next_available_stream_id(False)
-        stream = TrioQuicStream(self, stream_id)
-        self._streams[stream_id] = stream
-        return stream
+    async def make_stream(self, timeout=None):
+        if timeout is None:
+            context = NullContext(None)
+        else:
+            context = trio.move_on_after(timeout)
+        with context:
+            await self._handshake_complete.wait()
+            if self._done:
+                raise UnexpectedEOF
+            stream_id = self._connection.get_next_available_stream_id(False)
+            stream = TrioQuicStream(self, stream_id)
+            self._streams[stream_id] = stream
+            return stream
+        raise dns.exception.Timeout
 
     async def close(self):
         if not self._closed:
             self._manager.closed(self._peer[0], self._peer[1])
             self._closed = True
             self._connection.close()
             if self._worker_scope is not None:
```

### Comparing `dnspython-2.4.0rc1/dns/rcode.py` & `dnspython-2.4.1/dns/rcode.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdata.py` & `dnspython-2.4.1/dns/rdata.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdataclass.py` & `dnspython-2.4.1/dns/rdataclass.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdataset.py` & `dnspython-2.4.1/dns/rdataset.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdatatype.py` & `dnspython-2.4.1/dns/rdatatype.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/ANY/AFSDB.py` & `dnspython-2.4.1/dns/rdtypes/ANY/AFSDB.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/ANY/AMTRELAY.py` & `dnspython-2.4.1/dns/rdtypes/ANY/AMTRELAY.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/ANY/AVC.py` & `dnspython-2.4.1/dns/rdtypes/ANY/AVC.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/ANY/CAA.py` & `dnspython-2.4.1/dns/rdtypes/ANY/CAA.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/ANY/CDNSKEY.py` & `dnspython-2.4.1/dns/rdtypes/ANY/CDNSKEY.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/ANY/CDS.py` & `dnspython-2.4.1/dns/rdtypes/ANY/CDS.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/ANY/CERT.py` & `dnspython-2.4.1/dns/rdtypes/ANY/CERT.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/ANY/CNAME.py` & `dnspython-2.4.1/dns/rdtypes/ANY/CNAME.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/ANY/CSYNC.py` & `dnspython-2.4.1/dns/rdtypes/ANY/CSYNC.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/ANY/DLV.py` & `dnspython-2.4.1/dns/rdtypes/ANY/DLV.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/ANY/DNAME.py` & `dnspython-2.4.1/dns/rdtypes/ANY/DNAME.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/ANY/DNSKEY.py` & `dnspython-2.4.1/dns/rdtypes/ANY/DNSKEY.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/ANY/DS.py` & `dnspython-2.4.1/dns/rdtypes/ANY/DS.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/ANY/EUI48.py` & `dnspython-2.4.1/dns/rdtypes/ANY/EUI48.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/ANY/EUI64.py` & `dnspython-2.4.1/dns/rdtypes/ANY/EUI64.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/ANY/GPOS.py` & `dnspython-2.4.1/dns/rdtypes/ANY/GPOS.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/ANY/HINFO.py` & `dnspython-2.4.1/dns/rdtypes/ANY/HINFO.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/ANY/HIP.py` & `dnspython-2.4.1/dns/rdtypes/ANY/HIP.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/ANY/ISDN.py` & `dnspython-2.4.1/dns/rdtypes/ANY/ISDN.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/ANY/L32.py` & `dnspython-2.4.1/dns/rdtypes/ANY/L32.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/ANY/L64.py` & `dnspython-2.4.1/dns/rdtypes/ANY/L64.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/ANY/LOC.py` & `dnspython-2.4.1/dns/rdtypes/ANY/LOC.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/ANY/LP.py` & `dnspython-2.4.1/dns/rdtypes/ANY/LP.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/ANY/MX.py` & `dnspython-2.4.1/dns/rdtypes/ANY/MX.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/ANY/NID.py` & `dnspython-2.4.1/dns/rdtypes/ANY/NID.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/ANY/NINFO.py` & `dnspython-2.4.1/dns/rdtypes/ANY/NINFO.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/ANY/NS.py` & `dnspython-2.4.1/dns/rdtypes/ANY/NS.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/ANY/NSEC.py` & `dnspython-2.4.1/dns/rdtypes/ANY/NSEC.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/ANY/NSEC3.py` & `dnspython-2.4.1/dns/rdtypes/ANY/NSEC3.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/ANY/NSEC3PARAM.py` & `dnspython-2.4.1/dns/rdtypes/ANY/NSEC3PARAM.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/ANY/OPENPGPKEY.py` & `dnspython-2.4.1/dns/rdtypes/ANY/OPENPGPKEY.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/ANY/OPT.py` & `dnspython-2.4.1/dns/rdtypes/ANY/OPT.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/ANY/PTR.py` & `dnspython-2.4.1/dns/rdtypes/ANY/PTR.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/ANY/RP.py` & `dnspython-2.4.1/dns/rdtypes/ANY/RP.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/ANY/RRSIG.py` & `dnspython-2.4.1/dns/rdtypes/ANY/RRSIG.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/ANY/RT.py` & `dnspython-2.4.1/dns/rdtypes/ANY/RT.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/ANY/SOA.py` & `dnspython-2.4.1/dns/rdtypes/ANY/SOA.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/ANY/SPF.py` & `dnspython-2.4.1/dns/rdtypes/ANY/SPF.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/ANY/SSHFP.py` & `dnspython-2.4.1/dns/rdtypes/ANY/SSHFP.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/ANY/TKEY.py` & `dnspython-2.4.1/dns/rdtypes/ANY/TKEY.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/ANY/TSIG.py` & `dnspython-2.4.1/dns/rdtypes/ANY/TSIG.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/ANY/TXT.py` & `dnspython-2.4.1/dns/rdtypes/ANY/TXT.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/ANY/URI.py` & `dnspython-2.4.1/dns/rdtypes/ANY/URI.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/ANY/X25.py` & `dnspython-2.4.1/dns/rdtypes/ANY/X25.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/ANY/ZONEMD.py` & `dnspython-2.4.1/dns/rdtypes/ANY/ZONEMD.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/ANY/__init__.py` & `dnspython-2.4.1/dns/rdtypes/ANY/__init__.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/CH/A.py` & `dnspython-2.4.1/dns/rdtypes/CH/A.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/CH/__init__.py` & `dnspython-2.4.1/dns/rdtypes/CH/__init__.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/IN/A.py` & `dnspython-2.4.1/dns/rdtypes/IN/A.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/IN/AAAA.py` & `dnspython-2.4.1/dns/rdtypes/IN/AAAA.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/IN/APL.py` & `dnspython-2.4.1/dns/rdtypes/IN/APL.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/IN/DHCID.py` & `dnspython-2.4.1/dns/rdtypes/IN/DHCID.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/IN/IPSECKEY.py` & `dnspython-2.4.1/dns/rdtypes/IN/IPSECKEY.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/IN/KX.py` & `dnspython-2.4.1/dns/rdtypes/IN/KX.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/IN/NAPTR.py` & `dnspython-2.4.1/dns/rdtypes/IN/NAPTR.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/IN/NSAP.py` & `dnspython-2.4.1/dns/rdtypes/IN/NSAP.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/IN/NSAP_PTR.py` & `dnspython-2.4.1/dns/rdtypes/IN/NSAP_PTR.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/IN/PX.py` & `dnspython-2.4.1/dns/rdtypes/IN/PX.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/IN/SRV.py` & `dnspython-2.4.1/dns/rdtypes/IN/SRV.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/IN/WKS.py` & `dnspython-2.4.1/dns/rdtypes/IN/WKS.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/IN/__init__.py` & `dnspython-2.4.1/dns/rdtypes/IN/__init__.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/__init__.py` & `dnspython-2.4.1/dns/rdtypes/__init__.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/dnskeybase.py` & `dnspython-2.4.1/dns/rdtypes/dnskeybase.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/dsbase.py` & `dnspython-2.4.1/dns/rdtypes/dsbase.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/euibase.py` & `dnspython-2.4.1/dns/rdtypes/euibase.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/mxbase.py` & `dnspython-2.4.1/dns/rdtypes/mxbase.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/nsbase.py` & `dnspython-2.4.1/dns/rdtypes/nsbase.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/svcbbase.py` & `dnspython-2.4.1/dns/rdtypes/svcbbase.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/tlsabase.py` & `dnspython-2.4.1/dns/rdtypes/tlsabase.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/txtbase.py` & `dnspython-2.4.1/dns/rdtypes/txtbase.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rdtypes/util.py` & `dnspython-2.4.1/dns/rdtypes/util.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/renderer.py` & `dnspython-2.4.1/dns/renderer.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/resolver.py` & `dnspython-2.4.1/dns/resolver.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import contextlib
 import random
 import socket
 import sys
 import threading
 import time
 import warnings
-from typing import Any, Dict, Iterator, List, Optional, Tuple, Union
+from typing import Any, Dict, Iterator, List, Optional, Sequence, Tuple, Union
 from urllib.parse import urlparse
 
 import dns._ddr
 import dns.edns
 import dns.exception
 import dns.flags
 import dns.inet
@@ -916,15 +916,15 @@
     ednsoptions: Optional[List[dns.edns.Option]]
     payload: int
     cache: Any
     flags: Optional[int]
     retry_servfail: bool
     rotate: bool
     ndots: Optional[int]
-    _nameservers: List[Union[str, dns.nameserver.Nameserver]]
+    _nameservers: Sequence[Union[str, dns.nameserver.Nameserver]]
 
     def __init__(
         self, filename: str = "/etc/resolv.conf", configure: bool = True
     ) -> None:
         """*filename*, a ``str`` or file object, specifying a file
         in standard /etc/resolv.conf format.  This parameter is meaningful
         only when *configure* is true and the platform is POSIX.
@@ -1172,15 +1172,15 @@
         """
 
         self.flags = flags
 
     @classmethod
     def _enrich_nameservers(
         cls,
-        nameservers: List[Union[str, dns.nameserver.Nameserver]],
+        nameservers: Sequence[Union[str, dns.nameserver.Nameserver]],
         nameserver_ports: Dict[str, int],
         default_port: int,
     ) -> List[dns.nameserver.Nameserver]:
         enriched_nameservers = []
         if isinstance(nameservers, list):
             for nameserver in nameservers:
                 enriched_nameserver: dns.nameserver.Nameserver
@@ -1210,20 +1210,20 @@
                 )
             )
         return enriched_nameservers
 
     @property
     def nameservers(
         self,
-    ) -> List[Union[str, dns.nameserver.Nameserver]]:
+    ) -> Sequence[Union[str, dns.nameserver.Nameserver]]:
         return self._nameservers
 
     @nameservers.setter
     def nameservers(
-        self, nameservers: List[Union[str, dns.nameserver.Nameserver]]
+        self, nameservers: Sequence[Union[str, dns.nameserver.Nameserver]]
     ) -> None:
         """
         *nameservers*, a ``list`` of nameservers, where a nameserver is either
         a string interpretable as a nameserver, or a ``dns.nameserver.Nameserver``
         instance.
 
         Raises ``ValueError`` if *nameservers* is not a list of nameservers.
```

### Comparing `dnspython-2.4.0rc1/dns/reversename.py` & `dnspython-2.4.1/dns/reversename.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/rrset.py` & `dnspython-2.4.1/dns/rrset.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/serial.py` & `dnspython-2.4.1/dns/serial.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/set.py` & `dnspython-2.4.1/dns/set.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/tokenizer.py` & `dnspython-2.4.1/dns/tokenizer.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/transaction.py` & `dnspython-2.4.1/dns/transaction.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/tsig.py` & `dnspython-2.4.1/dns/tsig.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/tsigkeyring.py` & `dnspython-2.4.1/dns/tsigkeyring.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/ttl.py` & `dnspython-2.4.1/dns/ttl.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/update.py` & `dnspython-2.4.1/dns/update.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/version.py` & `dnspython-2.4.1/dns/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,19 +18,19 @@
 """dnspython release version information."""
 
 #: MAJOR
 MAJOR = 2
 #: MINOR
 MINOR = 4
 #: MICRO
-MICRO = 0
+MICRO = 1
 #: RELEASELEVEL
-RELEASELEVEL = 0x0C
+RELEASELEVEL = 0x0F
 #: SERIAL
-SERIAL = 1
+SERIAL = 0
 
 if RELEASELEVEL == 0x0F:  # pragma: no cover  lgtm[py/unreachable-statement]
     #: version
     version = "%d.%d.%d" % (MAJOR, MINOR, MICRO)  # lgtm[py/unreachable-statement]
 elif RELEASELEVEL == 0x00:  # pragma: no cover  lgtm[py/unreachable-statement]
     version = "%d.%d.%ddev%d" % (
         MAJOR,
```

### Comparing `dnspython-2.4.0rc1/dns/versioned.py` & `dnspython-2.4.1/dns/versioned.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/win32util.py` & `dnspython-2.4.1/dns/win32util.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,25 +202,23 @@
 
         def get(self):
             """Extract resolver configuration from the Windows registry."""
 
             lm = winreg.ConnectRegistry(None, winreg.HKEY_LOCAL_MACHINE)
             try:
                 tcp_params = winreg.OpenKey(
-                    lm, r"SYSTEM\CurrentControlSet" r"\Services\Tcpip\Parameters"
+                    lm, r"SYSTEM\CurrentControlSet\Services\Tcpip\Parameters"
                 )
                 try:
                     self._config_fromkey(tcp_params, True)
                 finally:
                     tcp_params.Close()
                 interfaces = winreg.OpenKey(
                     lm,
-                    r"SYSTEM\CurrentControlSet"
-                    r"\Services\Tcpip\Parameters"
-                    r"\Interfaces",
+                    r"SYSTEM\CurrentControlSet\Services\Tcpip\Parameters\Interfaces",
                 )
                 try:
                     i = 0
                     while True:
                         try:
                             guid = winreg.EnumKey(interfaces, i)
                             i += 1
```

### Comparing `dnspython-2.4.0rc1/dns/wire.py` & `dnspython-2.4.1/dns/wire.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/xfr.py` & `dnspython-2.4.1/dns/xfr.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/zone.py` & `dnspython-2.4.1/dns/zone.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/zonefile.py` & `dnspython-2.4.1/dns/zonefile.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/dns/zonetypes.py` & `dnspython-2.4.1/dns/zonetypes.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/examples/async_dns.py` & `dnspython-2.4.1/examples/async_dns.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/examples/ddns.py` & `dnspython-2.4.1/examples/ddns.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/examples/ddr.py` & `dnspython-2.4.1/examples/ddr.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/examples/doh-json.py` & `dnspython-2.4.1/examples/doh-json.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/examples/doh.py` & `dnspython-2.4.1/examples/doh.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/examples/doq.py` & `dnspython-2.4.1/examples/doq.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/examples/edns.py` & `dnspython-2.4.1/examples/edns.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/examples/edns_resolver.py` & `dnspython-2.4.1/examples/edns_resolver.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/examples/query_specific.py` & `dnspython-2.4.1/examples/query_specific.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/examples/receive_notify.py` & `dnspython-2.4.1/examples/receive_notify.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/examples/reverse.py` & `dnspython-2.4.1/examples/reverse.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/examples/zonediff.py` & `dnspython-2.4.1/examples/zonediff.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/pyproject.toml` & `dnspython-2.4.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dnspython"
-version = "2.4.0rc1"
+version = "2.4.1"
 description = "DNS toolkit"
 authors = ["Bob Halley <halley@dnspython.org>"]
 license = "ISC"
 packages = [
     {include = "dns"}
 ]
 include = [
@@ -35,20 +35,20 @@
 documentation = "https://dnspython.readthedocs.io/en/stable/"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/rthalley/dnspython/issues"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-httpx = {version=">=0.21.1", optional=true, python=">=3.6.2"}
-h2 = {version=">=4.1.0", optional=true, python=">=3.6.2"}
+httpx = {version=">=0.24.1", optional=true}
+httpcore = {version=">=0.17.3", optional=true}
+h2 = {version=">=4.1.0", optional=true}
 idna = {version=">=2.1,<4.0", optional=true}
 cryptography = {version=">=2.6,<42.0", optional=true}
 trio = {version=">=0.14,<0.23", optional=true}
-sniffio = {version="^1.1", optional=true}
 wmi = {version="^1.5.1", optional=true}
 aioquic = {version=">=0.9.20", optional=true}
 
 [tool.poetry.dev-dependencies]
 pytest = ">=5.4.1,<8"
 pytest-cov = "^4.0.0"
 flake8 = "^5.0.3"
@@ -57,15 +57,15 @@
 twine = "^4.0.0"
 wheel = "^0.40.0"
 pylint = "^2.7.4"
 mypy = ">=1.0.1"
 black = "^23.1.0"
 
 [tool.poetry.extras]
-doh = ['httpx', 'h2']
+doh = ['httpx', 'h2', 'httpcore']
 idna = ['idna']
 dnssec = ['cryptography']
 trio = ['trio']
 wmi = ['wmi']
 doq = ['aioquic']
 
 [build-system]
```

### Comparing `dnspython-2.4.0rc1/setup.cfg` & `dnspython-2.4.1/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dnspython
-version = 2.4.0rc1
+version = 2.4.1
 author = Bob Halley
 author_email = halley@dnspython.org
 license = ISC
 license_file = LICENSE
 description = DNS toolkit
 url = https://www.dnspython.org
 project_urls =
```

### Comparing `dnspython-2.4.0rc1/tests/example` & `dnspython-2.4.1/tests/example`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/tests/example1.good` & `dnspython-2.4.1/tests/example1.good`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/tests/example2.good` & `dnspython-2.4.1/tests/example2.good`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/tests/example3.good` & `dnspython-2.4.1/tests/example3.good`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/tests/example4.good` & `dnspython-2.4.1/tests/example4.good`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/tests/keys.py` & `dnspython-2.4.1/tests/keys.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/tests/nanonameserver.py` & `dnspython-2.4.1/tests/nanonameserver.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/tests/nanoquic.py` & `dnspython-2.4.1/tests/nanoquic.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,14 @@
     import aioquic.asyncio.server
     import aioquic.quic.configuration
     import aioquic.quic.events
 
     import dns.asyncquery
     import dns.message
     import dns.rcode
-
     from tests.util import here
 
     have_quic = True
 
     class Request:
         def __init__(self, message, wire):
             self.message = message
@@ -75,26 +74,28 @@
                 except Exception:
                     response = dns.message.make_response(q)
                     response.set_rcode(dns.rcode.SERVFAIL)
             wire = response.to_wire()
             return struct.pack("!H", len(wire)) + wire
 
     class Server(threading.Thread):
-        def __init__(self):
+        def __init__(self, address="127.0.0.1"):
             super().__init__()
+            self.address = address
             self.transport = None
             self.protocol = None
             self.left = None
             self.right = None
             self.ready = threading.Event()
 
         def __enter__(self):
             self.left, self.right = socket.socketpair()
             self.start()
             self.ready.wait(4)
+            return self
 
         def __exit__(self, ex_ty, ex_va, ex_tr):
             if self.protocol is not None:
                 self.protocol.close()
             if self.transport is not None:
                 self.transport.close()
             if self.left:
@@ -112,16 +113,18 @@
             )
             conf.load_cert_chain(here("tls/public.crt"), here("tls/private.pem"))
             loop = asyncio.get_event_loop()
             (self.transport, self.protocol) = await loop.create_datagram_endpoint(
                 lambda: aioquic.asyncio.server.QuicServer(
                     configuration=conf, create_protocol=NanoQuic
                 ),
-                local_addr=("127.0.0.1", 8853),
+                local_addr=(self.address, 0),
             )
+            info = self.transport.get_extra_info("sockname")
+            self.port = info[1]
             self.ready.set()
             try:
                 await reader.read(1)
             except Exception:
                 pass
 
         def run(self):
```

### Comparing `dnspython-2.4.0rc1/tests/svcb_test_vectors.generic` & `dnspython-2.4.1/tests/svcb_test_vectors.generic`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/tests/svcb_test_vectors.text` & `dnspython-2.4.1/tests/svcb_test_vectors.text`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/tests/test_address.py` & `dnspython-2.4.1/tests/test_address.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/tests/test_async.py` & `dnspython-2.4.1/tests/test_async.py`

 * *Files 3% similar despite different names*

```diff
@@ -405,14 +405,36 @@
             )
             self.assertTrue(rrs is not None)
             seen = set([rdata.address for rdata in rrs])
             self.assertTrue("8.8.8.8" in seen)
             self.assertTrue("8.8.4.4" in seen)
 
     @unittest.skipIf(not _ssl_available, "SSL not available")
+    def testQueryTLSWithContext(self):
+        for address in query_addresses:
+            qname = dns.name.from_text("dns.google.")
+
+            async def run():
+                ssl_context = ssl.create_default_context()
+                ssl_context.check_hostname = True
+                q = dns.message.make_query(qname, dns.rdatatype.A)
+                return await dns.asyncquery.tls(
+                    q, address, timeout=2, ssl_context=ssl_context
+                )
+
+            response = self.async_run(run)
+            rrs = response.get_rrset(
+                response.answer, qname, dns.rdataclass.IN, dns.rdatatype.A
+            )
+            self.assertTrue(rrs is not None)
+            seen = set([rdata.address for rdata in rrs])
+            self.assertTrue("8.8.8.8" in seen)
+            self.assertTrue("8.8.4.4" in seen)
+
+    @unittest.skipIf(not _ssl_available, "SSL not available")
     def testQueryTLSWithSocket(self):
         for address in query_addresses:
             qname = dns.name.from_text("dns.google.")
 
             async def run():
                 ssl_context = ssl.create_default_context()
                 ssl_context.check_hostname = False
@@ -636,16 +658,16 @@
                 except Exception:
                     self.assertTrue(False)
 
         self.async_run(run)
 
 
 try:
-    import trio
     import sniffio
+    import trio
 
     class TrioAsyncDetectionTests(AsyncDetectionTests):
         sniff_result = "trio"
 
         def async_run(self, afunc):
             return trio.run(afunc)
```

### Comparing `dnspython-2.4.0rc1/tests/test_bugs.py` & `dnspython-2.4.1/tests/test_bugs.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/tests/test_constants.py` & `dnspython-2.4.1/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/tests/test_ddr.py` & `dnspython-2.4.1/tests/test_ddr.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/tests/test_dnssec.py` & `dnspython-2.4.1/tests/test_dnssec.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,40 +11,40 @@
 # WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
 # MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL NOMINUM BE LIABLE FOR
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
-from datetime import datetime, timedelta, timezone
-from typing import Any
-
 import functools
+import time
 import unittest
+from datetime import datetime, timedelta, timezone
+from typing import Any
 
 import dns.dnssec
 import dns.name
 import dns.rdata
 import dns.rdataclass
+import dns.rdataset
 import dns.rdatatype
 import dns.rdtypes.ANY.CDNSKEY
 import dns.rdtypes.ANY.CDS
 import dns.rdtypes.ANY.DNSKEY
 import dns.rdtypes.ANY.DS
 import dns.rrset
 import dns.zone
-
 from dns.rdtypes.dnskeybase import Flag
 
 from .keys import test_dnskeys
 
 try:
     from cryptography.hazmat.backends import default_backend
+    from cryptography.hazmat.primitives.asymmetric import dsa, ec, ed448, ed25519, rsa
     from cryptography.hazmat.primitives.serialization import load_pem_private_key
-    from cryptography.hazmat.primitives.asymmetric import dsa, ec, ed25519, ed448, rsa
 except ImportError:
     pass  # Cryptography ImportError already handled in dns.dnssec
 
 # pylint: disable=line-too-long
 
 abs_dnspython_org = dns.name.from_text("dnspython.org")
 
@@ -918,14 +918,45 @@
                 rsasha512_ns,
                 unknown_alg_ns_rrsig,
                 unknown_alg_keys,
                 None,
                 rsasha512_when,
             )
 
+    def check_candidates(self, flags, protocol, expected_number_of_candidates):
+        algorithm = dns.dnssec.Algorithm.ED25519
+        zsk_private_key = ed25519.Ed25519PrivateKey.generate()
+        zsk_dnskey = dns.dnssec.make_dnskey(
+            public_key=zsk_private_key.public_key(),
+            algorithm=algorithm,
+            flags=flags,
+            protocol=protocol,
+        )
+        zsk_dnskey_rdataset = dns.rdataset.from_rdata(300, zsk_dnskey)
+        signer = dns.name.from_text("example")
+        a_rrset = dns.rrset.from_text(signer, 300, "IN", "A", "10.0.0.1")
+        inception = time.time()
+        expiration = inception + 86400
+        a_rrsig = dns.dnssec.sign(
+            a_rrset, zsk_private_key, signer, zsk_dnskey, inception, expiration
+        )
+        candidates = dns.dnssec._find_candidate_keys(
+            {signer: zsk_dnskey_rdataset}, a_rrsig
+        )
+        self.assertTrue(len(candidates) == expected_number_of_candidates)
+
+    def testCandidateKeyMustBeProtocol3(self):
+        self.check_candidates(Flag.ZONE, 1, 0)
+
+    def testCandidateKeyMustHaveZoneFlag(self):
+        self.check_candidates(0, 3, 0)
+
+    def testGoodCandidateKeyIsFound(self):
+        self.check_candidates(Flag.ZONE, 3, 1)
+
 
 @unittest.skipUnless(dns.dnssec._have_pyca, "Python Cryptography cannot be imported")
 class DNSSECMiscTestCase(unittest.TestCase):
     def testDigestToBig(self):
         with self.assertRaises(ValueError):
             dns.dnssec.DSDigest.make(256)
```

### Comparing `dnspython-2.4.0rc1/tests/test_dnssecalgs.py` & `dnspython-2.4.1/tests/test_dnssecalgs.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/tests/test_doh.py` & `dnspython-2.4.1/tests/test_doh.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 # THE SOFTWARE IS PROVIDED "AS IS" AND NOMINUM DISCLAIMS ALL WARRANTIES
 # WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
 # MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL NOMINUM BE LIABLE FOR
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
-import unittest
 import random
 import socket
+import unittest
 
 try:
     import ssl
 
     _have_ssl = True
 except Exception:
     _have_ssl = False
@@ -143,34 +143,37 @@
             nameserver_ip = random.choice(resolver_v6_addresses)
             q = dns.message.make_query("example.com.", dns.rdatatype.A)
             r = dns.query.https(
                 q, nameserver_ip, session=self.session, post=False, timeout=4
             )
             self.assertTrue(q.is_response(r))
 
-    def test_bootstrap_address_fails(self):
-        # We test this to see if v4 is available
-        if resolver_v4_addresses:
-            ip = "185.228.168.168"
-            invalid_tls_url = "https://{}/doh/family-filter/".format(ip)
-            valid_tls_url = "https://doh.cleanbrowsing.org/doh/family-filter/"
-            q = dns.message.make_query("example.com.", dns.rdatatype.A)
-            # make sure CleanBrowsing's IP address will fail TLS certificate
-            # check.
-            with self.assertRaises(httpx.ConnectError):
-                dns.query.https(q, invalid_tls_url, session=self.session, timeout=4)
-            # And if we don't mangle the URL, it should work.
-            r = dns.query.https(
-                q,
-                valid_tls_url,
-                session=self.session,
-                bootstrap_address=ip,
-                timeout=4,
-            )
-            self.assertTrue(q.is_response(r))
+    # This test is temporarily disabled as there's an expired certificate issue on one
+    # of the servers, so it fails on the part that is supposed to succeed (2023-07-15).
+
+    # def test_bootstrap_address_fails(self):
+    #     # We test this to see if v4 is available
+    #     if resolver_v4_addresses:
+    #         ip = "185.228.168.168"
+    #         invalid_tls_url = "https://{}/doh/family-filter/".format(ip)
+    #         valid_tls_url = "https://doh.cleanbrowsing.org/doh/family-filter/"
+    #         q = dns.message.make_query("example.com.", dns.rdatatype.A)
+    #         # make sure CleanBrowsing's IP address will fail TLS certificate
+    #         # check.
+    #         with self.assertRaises(httpx.ConnectError):
+    #             dns.query.https(q, invalid_tls_url, session=self.session, timeout=4)
+    #         # And if we don't mangle the URL, it should work.
+    #         r = dns.query.https(
+    #             q,
+    #             valid_tls_url,
+    #             session=self.session,
+    #             bootstrap_address=ip,
+    #             timeout=4,
+    #         )
+    #         self.assertTrue(q.is_response(r))
 
     def test_new_session(self):
         nameserver_url = random.choice(KNOWN_ANYCAST_DOH_RESOLVER_URLS)
         q = dns.message.make_query("example.com.", dns.rdatatype.A)
         r = dns.query.https(q, nameserver_url, timeout=4)
         self.assertTrue(q.is_response(r))
```

### Comparing `dnspython-2.4.0rc1/tests/test_edns.py` & `dnspython-2.4.1/tests/test_edns.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/tests/test_entropy.py` & `dnspython-2.4.1/tests/test_entropy.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/tests/test_exceptions.py` & `dnspython-2.4.1/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/tests/test_flags.py` & `dnspython-2.4.1/tests/test_flags.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/tests/test_generate.py` & `dnspython-2.4.1/tests/test_generate.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/tests/test_grange.py` & `dnspython-2.4.1/tests/test_grange.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/tests/test_immutable.py` & `dnspython-2.4.1/tests/test_immutable.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/tests/test_message.py` & `dnspython-2.4.1/tests/test_message.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/tests/test_name.py` & `dnspython-2.4.1/tests/test_name.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/tests/test_namedict.py` & `dnspython-2.4.1/tests/test_namedict.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/tests/test_nsec3.py` & `dnspython-2.4.1/tests/test_nsec3.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/tests/test_nsec3_hash.py` & `dnspython-2.4.1/tests/test_nsec3_hash.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/tests/test_ntoaaton.py` & `dnspython-2.4.1/tests/test_ntoaaton.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/tests/test_processing_order.py` & `dnspython-2.4.1/tests/test_processing_order.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/tests/test_query.py` & `dnspython-2.4.1/tests/test_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,17 +27,17 @@
 except Exception:
     have_ssl = False
 
 import dns.exception
 import dns.inet
 import dns.message
 import dns.name
+import dns.query
 import dns.rdataclass
 import dns.rdatatype
-import dns.query
 import dns.tsigkeyring
 import dns.zone
 import tests.util
 
 # Some tests use a "nano nameserver" for testing.  It requires trio
 # and threading, so try to import it and if it doesn't work, skip
 # those tests.
@@ -135,14 +135,30 @@
             rrs = response.get_rrset(
                 response.answer, qname, dns.rdataclass.IN, dns.rdatatype.A
             )
             self.assertTrue(rrs is not None)
             seen = set([rdata.address for rdata in rrs])
             self.assertTrue("8.8.8.8" in seen)
             self.assertTrue("8.8.4.4" in seen)
+
+    @unittest.skipUnless(have_ssl, "No SSL support")
+    def testQueryTLSWithContext(self):
+        for address in query_addresses:
+            qname = dns.name.from_text("dns.google.")
+            q = dns.message.make_query(qname, dns.rdatatype.A)
+            ssl_context = ssl.create_default_context()
+            ssl_context.check_hostname = False
+            response = dns.query.tls(q, address, timeout=2, ssl_context=ssl_context)
+            rrs = response.get_rrset(
+                response.answer, qname, dns.rdataclass.IN, dns.rdatatype.A
+            )
+            self.assertTrue(rrs is not None)
+            seen = set([rdata.address for rdata in rrs])
+            self.assertTrue("8.8.8.8" in seen)
+            self.assertTrue("8.8.4.4" in seen)
 
     @unittest.skipUnless(have_ssl, "No SSL support")
     def testQueryTLSWithSocket(self):
         for address in query_addresses:
             with socket.socket(
                 dns.inet.af_for_address(address), socket.SOCK_STREAM
             ) as base_s:
```

### Comparing `dnspython-2.4.0rc1/tests/test_rdata.py` & `dnspython-2.4.1/tests/test_rdata.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/tests/test_rdataset.py` & `dnspython-2.4.1/tests/test_rdataset.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/tests/test_rdtypeandclass.py` & `dnspython-2.4.1/tests/test_rdtypeandclass.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/tests/test_rdtypeanydnskey.py` & `dnspython-2.4.1/tests/test_rdtypeanydnskey.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/tests/test_rdtypeanyeui.py` & `dnspython-2.4.1/tests/test_rdtypeanyeui.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/tests/test_rdtypeanyloc.py` & `dnspython-2.4.1/tests/test_rdtypeanyloc.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/tests/test_rdtypeanytkey.py` & `dnspython-2.4.1/tests/test_rdtypeanytkey.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/tests/test_renderer.py` & `dnspython-2.4.1/tests/test_renderer.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/tests/test_resolution.py` & `dnspython-2.4.1/tests/test_resolution.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/tests/test_resolver.py` & `dnspython-2.4.1/tests/test_resolver.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/tests/test_resolver_override.py` & `dnspython-2.4.1/tests/test_resolver_override.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/tests/test_rrset.py` & `dnspython-2.4.1/tests/test_rrset.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/tests/test_rrset_reader.py` & `dnspython-2.4.1/tests/test_rrset_reader.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/tests/test_serial.py` & `dnspython-2.4.1/tests/test_serial.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/tests/test_set.py` & `dnspython-2.4.1/tests/test_set.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/tests/test_svcb.py` & `dnspython-2.4.1/tests/test_svcb.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/tests/test_tokenizer.py` & `dnspython-2.4.1/tests/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/tests/test_transaction.py` & `dnspython-2.4.1/tests/test_transaction.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/tests/test_tsig.py` & `dnspython-2.4.1/tests/test_tsig.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/tests/test_tsigkeyring.py` & `dnspython-2.4.1/tests/test_tsigkeyring.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/tests/test_ttl.py` & `dnspython-2.4.1/tests/test_ttl.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/tests/test_update.py` & `dnspython-2.4.1/tests/test_update.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/tests/test_wire.py` & `dnspython-2.4.1/tests/test_wire.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/tests/test_xfr.py` & `dnspython-2.4.1/tests/test_xfr.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/tests/test_zone.py` & `dnspython-2.4.1/tests/test_zone.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/tests/test_zonedigest.py` & `dnspython-2.4.1/tests/test_zonedigest.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/tests/tls/ca.crt` & `dnspython-2.4.1/tests/tls/ca.crt`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/tests/tls/public.crt` & `dnspython-2.4.1/tests/tls/public.crt`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/tests/util.py` & `dnspython-2.4.1/tests/util.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/util/constants-tool` & `dnspython-2.4.1/util/constants-tool`

 * *Files identical despite different names*

### Comparing `dnspython-2.4.0rc1/PKG-INFO` & `dnspython-2.4.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnspython
-Version: 2.4.0rc1
+Version: 2.4.1
 Summary: DNS toolkit
 Home-page: https://www.dnspython.org
 License: ISC
 Author: Bob Halley
 Author-email: halley@dnspython.org
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved
@@ -17,18 +17,18 @@
 Provides-Extra: doh
 Provides-Extra: doq
 Provides-Extra: idna
 Provides-Extra: trio
 Provides-Extra: wmi
 Requires-Dist: aioquic (>=0.9.20) ; extra == "doq"
 Requires-Dist: cryptography (>=2.6,<42.0) ; extra == "dnssec"
-Requires-Dist: h2 (>=4.1.0) ; (python_full_version >= "3.6.2") and (extra == "doh")
-Requires-Dist: httpx (>=0.21.1) ; (python_full_version >= "3.6.2") and (extra == "doh")
+Requires-Dist: h2 (>=4.1.0) ; extra == "doh"
+Requires-Dist: httpcore (>=0.17.3) ; extra == "doh"
+Requires-Dist: httpx (>=0.24.1) ; extra == "doh"
 Requires-Dist: idna (>=2.1,<4.0) ; extra == "idna"
-Requires-Dist: sniffio (>=1.1,<2.0)
 Requires-Dist: trio (>=0.14,<0.23) ; extra == "trio"
 Requires-Dist: wmi (>=1.5.1,<2.0.0) ; extra == "wmi"
 Project-URL: Bug Tracker, https://github.com/rthalley/dnspython/issues
 Project-URL: Documentation, https://dnspython.readthedocs.io/en/stable/
 Project-URL: Repository, https://github.com/rthalley/dnspython.git
 Description-Content-Type: text/markdown
 
@@ -60,33 +60,35 @@
 `socket.gethostbyname()`.
 
 dnspython originated at Nominum where it was developed
 to facilitate the testing of DNS software.
 
 ## ABOUT THIS RELEASE
 
-This is dnspython 2.4.0rc1.
+This is dnspython 2.4.1.
 Please read
-[What's New](https://dnspython.readthedocs.io/en/latest/whatsnew.html) for
+[What's New](https://dnspython.readthedocs.io/en/stable/whatsnew.html) for
 information about the changes in this release.
 
 ## INSTALLATION
 
 * Many distributions have dnspython packaged for you, so you should
   check there first.
 * To use a wheel downloaded from PyPi, run:
 
     pip install dnspython
 
 * To install from the source code, go into the top-level of the source code
   and run:
 
+```
     pip install --upgrade pip build
     python -m build
     pip install dist/*.whl
+```
 
 * To install the latest from the master branch, run `pip install git+https://github.com/rthalley/dnspython.git`
 
 Dnspython's default installation does not depend on any modules other than
 those in the Python standard library.  To use some features, additional modules
 must be installed.  For convenience, pip options are defined for the
 requirements.
```

