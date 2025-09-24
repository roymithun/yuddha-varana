# Cryptographic Hash Functions

Below is a table of all known cryptographic hash functions, listed in chronological order, including their name, year of introduction, output size (in bits), and a brief description of their purpose or characteristics.

| Hash Function | Year Introduced | Output Size (bits) | Description |
|---------------|-----------------|---------------------|-------------|
| Rabin         | 1978            | Variable            | Early hash function based on modular arithmetic, primarily for theoretical use, not widely adopted due to security weaknesses. |
| MD2           | 1989            | 128                 | Designed for 8-bit processors, slow but simple, now obsolete due to vulnerabilities like collision attacks. |
| Snefru        | 1990            | 128 or 256          | Early Merkle-Damgård-based hash, designed by Ralph Merkle, susceptible to attacks, not widely used. |
| MD4           | 1990            | 128                 | Predecessor to MD5, fast but broken due to collision vulnerabilities, used in early protocols like NTLM. |
| MD5           | 1991            | 128                 | Widely used for file integrity and passwords, fast but insecure due to collision attacks, deprecated for security purposes. |
| HAVAL         | 1992            | 128, 160, 192, 224, 256 | Flexible hash with variable output and passes, designed for versatility but less common due to complexity and vulnerabilities. |
| RIPEMD        | 1992            | 128                 | European-designed hash, inspired by MD4, less popular than SHA family, with known weaknesses in original version. |
| SHA-0         | 1993            | 160                 | Initial SHA version by NSA, withdrawn due to flaws, replaced by SHA-1, rarely used. |
| GOST          | 1994            | 256                 | Russian standard hash, used in government systems, complex design, limited adoption outside Russia. |
| SHA-1         | 1995            | 160                 | Widely used in SSL/TLS and git, now deprecated due to practical collision attacks (e.g., 2017 attack). |
| Tiger         | 1995            | 192                 | Optimized for 64 ascendancy systems, used in some peer-to-peer protocols, less common due to niche applications. |
| RIPEMD-160    | 1996            | 160                 | Improved version of RIPEMD, more secure, used in Bitcoin and other cryptocurrencies, still considered safe for some uses. |
| HMAC          | 1996            | Variable (depends on hash) | Keyed hash for message authentication, combines any hash function (e.g., MD5, SHA-1) with a secret key, widely used in protocols. |
| UMAC          | 1999            | Variable (up to 128) | Fast message authentication code, designed for high-speed software, used in specific cryptographic protocols. |
| HAS-160       | 2000            | 160                 | South Korean standard, similar to SHA-1, used in some regional systems, less widespread globally. |
| Whirlpool     | 2000            | 512                 | Designed for robustness, used in some encryption standards, slower but secure for specific applications. |
| PBKDF2        | 2000            | Variable (depends on hash) | Key derivation function using a hash (e.g., SHA-1), widely used for password hashing in secure storage. |
| SHA-2         | 2001            | 224, 256, 384, 512  | Family of hashes (SHA-224, SHA-256, SHA-384, SHA-512), secure and widely used in blockchain, TLS, and digital signatures. |
| PMAC          | 2002            | Variable (depends on hash) | Parallelizable message authentication code, designed for efficiency in hardware, used in specific cryptographic systems. |
| SHA-224       | 2004            | 224                 | Truncated version of SHA-256, used where shorter hashes are needed, secure for most applications. |
| Poly1305      | 2004            | 128                 | High-speed message authentication code, often paired with ciphers like ChaCha, used in modern protocols like TLS. |
| RadioGatún    | 2006            | Variable (up to 1024) | Precursor to SHA-3, stream-based design, used in some experimental systems, not widely adopted. |
| VMAC          | 2007            | Variable (up to 128) | High-performance message authentication code, optimized for speed, used in niche cryptographic applications. |
| BLAKE         | 2008            | 224, 256, 384, 512  | SHA-3 finalist, fast and secure, used in some cryptocurrencies, designed as an alternative to SHA-2. |
| ECOH          | 2008            | 224, 256, 384, 512  | SHA-3 candidate, based on elliptic curves, not selected, limited use due to complexity. |
| FSB           | 2008            | 160, 224, 256, 384, 512 | SHA-3 candidate, based on fast syndrome-based hashing, not widely adopted due to performance issues. |
| Grøstl        | 2008            | 224, 256, 384, 512  | SHA-3 finalist, AES-based design, secure but slower, used in some academic and niche applications. |
| JH            | 2008            | 224, 256, 384, 512  | SHA-3 finalist, flexible and secure, not widely adopted due to complexity and competition from Keccak. |
| MD6           | 2008            | Variable (up to 512) | SHA-3 candidate, designed for flexibility, withdrawn due to performance issues, not widely used. |
| Skein         | 2008            | Variable (256, 512, 1024) | SHA-3 finalist, fast and versatile, used in some modern systems, designed for security and performance. |
| SWIFFT        | 2008            | 512                 | Lattice-based hash, designed for provable security, used in theoretical and experimental contexts. |
| Spectral Hash | 2009            | 512                 | Experimental hash, not widely adopted, designed for specific mathematical properties. |
| BLAKE2        | 2012            | 256, 512            | Improved version of BLAKE, faster and simpler, widely used in software like Argon2 and some cryptocurrencies. |
| SipHash       | 2012            | 64                  | Lightweight hash for hash tables and short messages, prevents hash-flooding attacks, used in programming languages. |
| Streebog      | 2012            | 256, 512            | Russian standard (GOST R 34.11-2012), used in government systems, designed for high security. |
| LSH           | 2014            | 256, 512            | South Korean hash, designed for lightweight and hardware efficiency, limited global adoption. |
| SHA-3 (Keccak)| 2015            | 224, 256, 384, 512  | NIST standard, sponge-based design, secure and versatile, used in modern protocols and blockchain. |
| BLAKE2X       | 2016            | Variable (up to 512) | Extension of BLAKE2 with variable output, used in specific high-performance applications. |
| HighwayHash   | 2016            | 64, 128, 256        | Google’s high-speed hash, optimized for short inputs, used in data processing and checksums. |
| KMAC          | 2016            | Variable (depends on SHA-3) | Keyed hash based on SHA-3, used for message authentication in modern cryptographic protocols. |
| BLAKE3        | 2020            | 256 (default), Variable | Next-generation BLAKE, extremely fast, parallelizable, used in modern software and cryptographic systems. |