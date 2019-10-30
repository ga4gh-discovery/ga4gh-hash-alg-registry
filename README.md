# GA4GH Discovery - Checksum Specification [![LICENCE](https://img.shields.io/github/license/ga4gh-discovery/ga4gh-checksum)](https://github.com/ga4gh-discovery/ga4gh-checksum/blob/master/LICENSE)

Checksums are core component of building reproducible computational workflows on verifying datasets. They are typically fixed size bit-strings generated by applying a checksum algorithm on a block of data to help verify the integrity of the data. The specification provides a reusable schema object definition to specify a checksum algorithm type and value.

This repository also hosts the GA4GH Hash Algorithm Registry that extends the [IANA Hash Algorithm Registry](https://www.iana.org/assignments/named-information/named-information.xhtml#hash-alg) with hash algorithms specific to the GA4GH community requirements.

## Specification

Checksum is described as a [SchemaBlock object](https://github.com/ga4gh-discovery/ga4gh-checksum/blob/master/checksum.yaml).

[GA4GH Hash Algorithm Registry](https://github.com/ga4gh-discovery/ga4gh-checksum/blob/master/hash-alg.csv)

| ID    | Hash Name String | Value Length   | Reference                                                                                   | Status  |
|:------|------------------|----------------|---------------------------------------------------------------------------------------------|---------|
| 0     | Reserved         |                | [RFC6920](http://www.iana.org/go/rfc6920)                                                   |         |
| 1     | sha-256          | 256 bits       | [RFC6920](http://www.iana.org/go/rfc6920)                                                   | current |
| 2     | sha-256-128      | 128 bits       | [RFC6920](http://www.iana.org/go/rfc6920)                                                   | current |
| 3     | sha-256-120      | 120 bits       | [RFC6920](http://www.iana.org/go/rfc6920)                                                   | current |
| 4     | sha-256-96       | 96 bits        | [RFC6920](http://www.iana.org/go/rfc6920)                                                   | current |
| 5     | sha-256-64       | 64 bits        | [RFC6920](http://www.iana.org/go/rfc6920)                                                   | current |
| 6     | sha-256-32       | 32 bits        | [RFC6920](http://www.iana.org/go/rfc6920)                                                   | current |
| 7     | sha-384          | 384 bits       | [FIPS 180-4](https://dx.doi.org/10.6028/NIST.FIPS.180-4)                                    | current |
| 8     | sha-512          | 512 bits       | [FIPS 180-4](https://dx.doi.org/10.6028/NIST.FIPS.180-4)                                    | current |
| 9     | sha3-224         | 224 bits       | [FIPS 202](https://dx.doi.org/10.6028/NIST.FIPS.202)                                        | current |
| 10    | sha3-256         | 256 bits       | [FIPS 202](https://dx.doi.org/10.6028/NIST.FIPS.202)                                        | current |
| 11    | sha3-384         | 384 bits       | [FIPS 202](https://dx.doi.org/10.6028/NIST.FIPS.202)                                        | current |
| 12    | sha3-512         | 512 bits       | [FIPS 202](https://dx.doi.org/10.6028/NIST.FIPS.202)                                        | current |
| 13    | md5              | 128 bits       | [RFC1321](https://www.ietf.org/rfc/rfc1321.txt)                                             | current |
| 14    | etag             | 128 + var bits | [RFC7232](https://tools.ietf.org/html/rfc7232#section-2.3)                                  | current |
| 15    | crc32c           | 32 bits        | [RFC4960](https://tools.ietf.org/html/rfc4960#appendix-B)                                   | current |
| 16    | trunc512         | 192 bits       | [GA4GH Refget](https://samtools.github.io/hts-specs/refget.html#trunc512-algorithm-details) | current |
| 17    | sha1             | 160 bits       | [FIPS 180-4](https://dx.doi.org/10.6028/NIST.FIPS.180-4)                                    | current |
| 18    | blake2b-512      | 512 bits       | [RFC7693](https://tools.ietf.org/html/rfc7693)                                              | current |
| 19-31 | Unassigned       |                |                                                                                             |         |
| 32    | Reserved         |                | [RFC6920](http://www.iana.org/go/rfc6920)                                                   |         |
| 33-63 | Unassigned       |                |                                                                                             |         |

## Contributing
The GA4GH is an open community that strives for inclusivity. Teleconferences and corresponding meeting minutes are open to the public. To learn how to contribute to this effort, please email Rishi Nag (rishi.nag@ga4gh.org).
