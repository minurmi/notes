
Clicked renew on the Digicert certificate order.
Generated a crs on alsin with the following command and input

```
openssl req -new -newkey rsa:4096 -nodes -keyout 20221010.4096.key -out cert_server_request.crs

-----
You are about to be asked to enter information that will be incorporated
into your certificate request.
What you are about to enter is what is called a Distinguished Name or a DN.
There are quite a few fields but you can leave some blank
For some fields there will be a default value,
If you enter '.', the field will be left blank.
-----
Country Name (2 letter code) [AU]:FI
State or Province Name (full name) [Some-State]:Uusimaa
Locality Name (eg, city) []:Espoo
Organization Name (eg, company) [Internet Widgits Pty Ltd]:PulseOn Oy
Organizational Unit Name (eg, section) []:
Common Name (e.g. server FQDN or YOUR name) []:*.ahjo.pulseon.fi
Email Address []:shady-ssl-certs@pulseon.fi
Please enter the following 'extra' attributes
to be sent with your certificate request
A challenge password []:
An optional company name []:
```

Copy-pasted the crs to DigiCert renewal page
selected DNS txt record as verification method
added credit card info and clicked order.
Asked Jari to place the magic text to the fi dns record


mv /home/ionakka/20211011.4096.key /etc/nginx/bad-place-for-keys/
ls -al /etc/nginx/bad-place-for-keys/
chown www-data:www-data /etc/nginx/bad-place-for-keys/20211011.4096.key
ls -al /etc/nginx/bad-place-for-keys/
ls /etc/ssl/certs/
ls -l /etc/ssl/certs/
ls -l /etc/ssl/certs/ | grep -v -e -\>
less /etc/ssl/certs/server-rapidssl-combo.crt
mv /home/ionakka/star_ahjo_pulseon_fi.pem /etc/ssl/certs/ahjo_digicert_$(date +%Y%m%d).pem
ls -l /etc/ssl/certs/ | grep -v -e -\>
chown root:root /etc/ssl/certs/ahjo_digicert_20211012.pem
ls -l /etc/nginx/bad-place-for-keys/20211011.4096.key
vi /etc/nginx/sites-enabled/default
vi /etc/nginx/sites-enabled/kristiina
vim.tiny /etc/nginx/sites-available/kristiina
service nginx restart
vim.tiny /etc/nginx/sites-available/kristiina
service nginx restart
ls -al /etc/nginx/sites-available/
ls -al /etc/nginx/sites-enabled/
diff -u /etc/nginx/sites-enabled/kristiina /etc/nginx/sites-available/kristiina
rm /etc/nginx/sites-enabled/kristiina
ln -s /etc/nginx/sites-available/kristiina /etc/nginx/sites-enabled/
ls -al /etc/nginx/sites-enabled/



ssl_certificate /etc/ssl/certs/ahjo_digicert_20211012.pem;
ssl_certificate_key /etc/nginx/bad-place-for-keys/20211011.4096.key;


-----BEGIN CERTIFICATE REQUEST-----
MIIFMDCCAxgCAQAwgaoxCzAJBgNVBAYTAkZJMRAwDgYDVQQIDAdVdXNpbWFhMQ4w
DAYDVQQHDAVFc3BvbzETMBEGA1UECgwKUHVsc2VPbiBPeTEdMBsGA1UECwwUU2hh
ZHkgU1NMIG9wZXJhdGlvbnMxGjAYBgNVBAMMESouYWhqby5wdWxzZW9uLmZpMSkw
JwYJKoZIhvcNAQkBFhpzaGFkeS1zc2wtY2VydHNAcHVsc2Vvbi5maTCCAiIwDQYJ
KoZIhvcNAQEBBQADggIPADCCAgoCggIBAM1dCYPKTfVTDUMbi5NLAxIEfko2C63B
Lipf1gGinFgjUZYEfANldUYAmNpqpMsNzpvWjJf7m9jzj1abKqShIlFgoFwqZOhP
bZ6AmxlXt9BLto1tZg0seEIf7R/xCLxRwh+W/bJDrlTHnSqlwRlgSx5BqnaQq1sc
HhyirJfLWGu/y60Sp+3e1AIq6+Ulh4aF9N92LN++8v0gWzqzgYY7yuBAAS/phA1V
6B5eyslRh4bBb09AoJduLyErUMneD7SGgeeBtWqzd2+YwkgRzp1fviLBbTL3Echw
rNLXKlGVKj1U2qA32WSuDTwAjO4wAo60uHNlahQv0Bq+IXdiPv6/C7wu4yLZOSJg
NNq5McGgl1YFAKH8GJZzG8gT51aD7+2CSOU3jAehONhH2xAN/usDFFZQGUnLwGCx
mL3BH14tJHQxeaEJUFjWj7ngS56iurTtJIEKcKoscP8Giz+OzrdkBJRNQrl1UIIJ
cInN7fhPd+ocr7JwECh563hEfybZN/PwFZSuFAhpXBqR0eE+pzx3fctNTsd5wLaG
P2rY1X7TaCiBTmWczWDJXiwUSHbOzjj8ETHFP6cMizH3Bf4FEc8zjwhlS7RliO0U
xOGfp9fiaYRxx/Xzmje2BdeXEhxrmEFPSncLyBavVmkQ6ojEw+9BlvxOdngKUYvv
1QGx75AVq3nFAgMBAAGgQDA+BgkqhkiG9w0BCQ4xMTAvMC0GA1UdEQQmMCSCD2Fo
am8ucHVsc2Vvbi5maYIRKi5haGpvLnB1bHNlb24uZmkwDQYJKoZIhvcNAQELBQAD
ggIBAFWuiT0bF+nPPGU+yKKJqyBbB/kesv55SspNSCi6d6szRN6NsITUsrq4u0iz
YckZe888oxetkvTANyDtDlhs+4SvB0xxgVi3B++7bvZL/OYv0VMtKbJZWq54kif5
xTMRYFg1FhjT1KoHglMwKM7RMIorksx5DCQMbOBU1NQuxND2CZNzyZVogRsZdPgp
FcUQ9K5Q1PbppXH+QtnBzsaEPCG1MNFAXmT2sDp0ErsngYrVQsXVLX5v6b+BoCK7
Odof4DY66iSuTwOzNHKPvePvC8Vlo3kZp1xj0N4uPhlWHVY5oVqXYReLJ00sO4+F
Gy+6ICbA56JWdNEzmwIQhcbNnbwsRvR1l6H1DMznyLedWMXMM3QVRZE6NtjQ0rY8
1oWZ8TAaaVvcslwISisMcXDd+RpHuT+0svKkTWBMhOhnkjijYw309DOa1bah8Jja
c+5jH0mApuSkNTyGPNL+YyH8PPdDnt8D92mpozGlzMP91Fp1PZwVunqymZd5Bv+7
NFP85fNJWfMmyUWcZQNBaxmUpMcrVUmfzfLtOqrtml34SRhKtQsT2rzMzS6eCEEs
u58qEzsP5UIH/9PofnQ2ZayIenro79X7SQXrfox6TVETiVqC8gGfHnXjUDuSyiFk
x3SObKVzAB87ZsjAshW6bfn+WNhipbVlpWS90VNPQ+mv/DyZ
-----END CERTIFICATE REQUEST-----


CSR Details
Common name
*.ahjo.pulseon.fi
City/locality: Espoo
Key algorithm
RSA
Organization: PulseOn Oy
State/province: Uusimaa
Key size: 4096
Country: FI
SANs:
ahjo.pulseon.fi
*.ahjo.pulseon.fi
