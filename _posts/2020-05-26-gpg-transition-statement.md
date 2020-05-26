---
layout: post
title: GPG transition statement
---

This exact same text can be found at [this location](/public/transition_statement_2020-05-26.txt).

```
-----BEGIN PGP SIGNED MESSAGE-----
Hash: SHA256

2020-05-26T04:33:53+00:00

For a number of reasons, i've recently set up a new OpenPGP key, and
will be transitioning away from my old one.

The old key will continue to be valid for some time, but i prefer all
future correspondence to come to the new one.  I would also like this
new key to be re-integrated into the web of trust.  This message is
signed by both keys to certify the transition.

the old key was:

pub   rsa2048/0x7504A77555E6B7CD 2015-06-07 [SC] [expires: 2020-06-05]
      Key fingerprint = 93BA 9F75 2110 BF46 4195  9608 7504 A775 55E6 B7CD
pub   rsa4096/0xC6F4103DB958A4B4 2016-09-24 [SC] [expires: 2021-09-23]                       
      Key fingerprint = 46C7 F5E6 2990 DDBE 57FF  2EAB C6F4 103D B958 A4B4

And the new key is:

pub   rsa4096/0x3CA48440DD473897 2020-05-26 [C]
      Key fingerprint = 1193 C2D2 E587 9FBF 7845  BBB4 3CA4 8440 DD47 3897

To fetch the full key you can get it with:

  wget -q -O- https://ycwan9.tk/pgp.txt | gpg --import -

Or, to fetch my new key from a public key server, you can simply do:

  gpg --keyserver pgp.mit.edu --recv-key 0x3CA48440DD473897

If you already know my old key, you can now verify that the new key is
signed by the old one:

  gpg --check-sigs 0x3CA48440DD473897

If you don't already know my old key, or you just want to be double
extra paranoid, you can check the fingerprint against the one above:

  gpg --fingerprint 0x3CA48440DD473897

If you are satisfied that you've got the right key, and the UIDs match
what you expect, I'd appreciate it if you would sign my key:

  gpg --sign-key 0x3CA48440DD473897

Lastly, if you could upload these signatures, i would appreciate it.
You can either send me an e-mail with the new signatures (if you have
a functional MTA on your system):

  gpg --armor --export 0x3CA48440DD473897 | mail -s 'OpenPGP Signatures' i at ycwan9.tk

Or you can just upload the signatures to a public keyserver directly:

  gpg --keyserver pgp.mit.edu --send-key 0x3CA48440DD473897

Please let me know if there is any trouble, and sorry for the
inconvenience.

Regards,
	ycwan9
-----BEGIN PGP SIGNATURE-----

iQIzBAEBCAAdFiEERsf15imQ3b5X/y6rxvQQPblYpLQFAl7Mp4gACgkQxvQQPblY
pLQwMA/+Mrf6tFOL7g2eeGMCn9fwXXzw2LuAMvTQmXvsrax734LwSw56PC7c2J/a
W3A5hNIhHR/fay9v0N0QLw6E1xu1E7SoEbryjWqDKMQ+6rt7W8+Y/WS76ZficrHP
LRzjBc1NnBr3hJN7KStnhJk6l1rwKYlx9Ub7Z6BZ8cAOAE/HPwHaVEjQ7Aqhhrls
V5ATbYtQJtTmk3OJnSRS5F4hXvLxzwVdU0m2P7QzViUS3FD7Byf8i/z3R3EyT5mW
9yuCcSS6DW4FnudYAxYCp2KwqWNv37TFa+FQraIF5WV3iVFmdPYnJhj4eBG2uejd
5IxIsjl46uL82y8uFECv5psEmtQlvGzseE3R9HIm7CouvHiqjmbWFLGviSzVW9z9
y1DwJSnd2TkX4ZTCiaPct2fyw7oaccavIDfBReUO3d4r+tm3TkVMEAw7vXHCTOXB
tWKksgOVcqZUg6a1hXI1xHceh2/u8poFr+N2MAaebYV01pKQ0UH0ZpCHOK+7e0/k
9tyy4Ngu2kFb+lyLWHaRQ7TM62pCoOrX1L1aTWZEdKQFMMK81icBv8Vcz+uhxm5C
6ropWF5Z4JgArpSX4B/tE4cUYSCZov/YFfKF42l7j2VNB8CLGDiMhEGzufqzCfia
ijHqAsmXISIWFHHAdj65DCmwLvwnYh7BByREXo+fgHLbN6s//vuJATMEAQEIAB0W
IQSTup91IRC/RkGVlgh1BKd1Vea3zQUCXsynjAAKCRB1BKd1Vea3zQhCCACoLWJP
ek0fOxakaxxpkz83TvhjjLJnSClqaCzIyUIH2tyLfaUyslGYTmczuQjzWaKblXt4
vVjnVSRGoisnxk4Wg9ayfo0pkifWs4xqMxnSTd7fZLLu/32nBY9DJSKps6BGcfjn
eaaRdplAav2wUC9myfMCjqRhB4ii+UP3IqQzE/tR04v0KJm0wiJCMMZQla+aElzb
EJ4UCjj14RwbsXKmWNeH4MpF7VZ1ZoO6ful3NVUuDDpNC/rzR8fZUMr3LmmlLvOq
gMXMDdRCNHrD39wlyBLlqyW/cJeR78E/01m7PCj6wUFi6Id2N/nYlEDD7l2/vrg0
HkFKCWWFXOiZkWguiQIzBAEBCAAdFiEEaWyvKtkXPslJ4f1Stl39o99nZyUFAl7M
p40ACgkQtl39o99nZyVzaxAAh1OFx3XslxhIcMolOAMp9hjU2Mixj5TuOpBUas91
p2lWt81N3lrivFUuGjnO/TZhUiMNxpq2DkBaWTJ9EFi6FG/Do0Rz041L199efbNi
wLfKuV2QlrM0NJ2cW2ksXKOrVxn/cgbGEtv/4wsD4sh1nzcvfO1O1ieAIk5jgQks
Hb+Zrjv0IMn2HX/m5O+jjIStzS6Qmov67wIR91xDY5u5CZu+GEDfNDbG1Riu1kwp
viy+mkWDtQ/V9ps2IRSp9GHrlHulT1qQ8Qrws6/I/Se7etivaBI3U6XGGqsOCbLS
Pe9scDGjixsYiCpG4LdnEqbmthXc2ZA20GF6KpXIpJY/VVehs3kR9YwUfAqd11rG
QFdpr3i6/mDy8SusALyXrDtBxKN7c8KioJK3MvDawT6Hy5e8sMyLDzTLTeXa5h6x
gYUeyhPdRZ33gfiBKRaWbQnlPU5692ZsOb90YuD7CCA/I3p9WX6MTgFjsPSeCFJX
fpmNz0vV0jd6YnSJCi+WiZScGJQlnWdPwCt4gdos9D/Dd3hrDFzPNFB8q3deFkm7
xvTlWVqTytdeuxoH4Gy2q2uiYGJhwCy4bFodm3st+2Hjl1ntWOAH5B7fiEt9XUdN
EAGSZXrovJSSzAPGN7AEKUA0Pt1D9IfWaJo0u3LtX8k+fQH6XUm3XKp7i2E0I/r8
GOI=
=xEiw
-----END PGP SIGNATURE-----
```
