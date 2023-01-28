## **Configurazione Test Merkle Tree**

+ Numero iterazioni: 500
+ Soglia: 0.5 --> con il 50% delle claims rivelate della VP

**TEST MERKLE TREE - Creazione e Verifica VC**  

| TEST |       Hl       |    HT     | NONCE | COMPRESSION PROOF | VC-issue (time,size, standard deviation) | VC-verify (time, standard deviation) |
| ---- | :------------: | :-------: | :---: | :---------------: | :--------------------------------------: | :----------------------------------: |
| 1    | HMAC-keccak256 | SHA3-256  |  256  |        NO         |    1-MT-VC-issue-Lkeccak-Tsha256.txt     |  1-MT-VC-verify-Lkeccak-Tsha256.txt  |
| 2    | HMAC-SHA3-256  | keccak256 |  256  |        NO         |    2-MT-VC-issue-Lsha256-Tkeccak.txt     |  2-MT-VC-verify-Lsha256-Tkeccak.txt  |
| 3    | HMAC-SHA3-256  | SHA3-512  |  256  |        NO         |    3-MT-VC-issue-Lsha256-Tsha512.txt     |  3-MT-VC-verify-Lsha256-Tsha512.txt  |



**TEST MERKLE TREE - Creazione e Verifica VP**

| TEST |       Hl       |    HT     | NONCE | COMPRESSION PROOF |    VP-issue (time,size, standard deviation)    |      VP-verify (time, standard deviation)      |
| :--: | :------------: | :-------: | :---: | :---------------: | :--------------------------------------------: | :--------------------------------------------: |
|  1   | HMAC-keccak256 | SHA3-256  |  256  |        NO         |       1-MT-VP-issue-Lkeccak-Tsha256.txt        |       1-MT-VP-verify-Lkeccak-Tsha256.txt       |
|  2   | HMAC-SHA3-256  | keccak256 |  256  |        NO         |       2-MT-VP-issue-Lsha256-Tkeccak.txt        |       2-MT-VP-verify-Lsha256-Tkeccak.txt       |
|  3   | HMAC-SHA3-256  | SHA3-512  |  256  |        NO         |       3-MT-VP-issue-Lsha256-Tsha512.txt        |       3-MT-VP-verify-Lsha256-Tsha512.txt       |
|  4   | HMAC-keccak256 | SHA3-256  |  256  |        SI         | 1-Compression-MT-VP-issue-Lkeccak-Tsha256.txt  | 1-Compression-MT-VP-verify-Lkeccak-Tsha256.txt |
|  5   | HMAC-SHA3-256  | keccak256 |  256  |        SI         | 2-Compression-MT-VP-issue-Lsha256-Tkeccak-.txt | 2-Compression-MT-VP-verify-Lsha256-Tkeccak.txt |
|  6   | HMAC-SHA3-256  | SHA3-512  |  256  |        SI         | 3-Compression-MT-VP-issue-Lsha256-Tsha512-.txt | 3-Compression-MT-VP-verify-Lsha256-Tsha512.txt |