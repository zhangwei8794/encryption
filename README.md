﻿# [encryption](https://github.com/qitas/encryption) 

#### qitas@qitas.cn

### [简介](https://github.com/Qitas/encryption/wiki)


## 组成

#### [AES对称加密](AES/)

对称加密在加密和解密过程中用到的密钥是相同的，这种加密方式加密速度非常快，适合经常发送数据的场合，其缺点是密钥的传输比较麻烦。

AES：Advanced Encryption Standard，又称Rijndael加密法，旨在取代DES成为广泛使用的标准，微信小程序加密传输采用该加密算法。

AES为分组密码，分组密码也就是把明文分成一组一组的，每组长度相等，每次加密一组数据，直到加密完整个明文。在AES标准规范中，分组长度只能是128位，也就是说，每个分组为16个字节（每个字节8位）。密钥的长度可以使用128位、192位或256位。密钥的长度不同，加密轮数也不同。

AES加密函数E，密文C = E(K, P),其中P为明文，K为密钥。
AES解密函数D，明文P = D(K, C),其中C为密文，K为密钥。

实际应用一般是通过RSA加密AES的密钥，传输到接收方，接收方解密得到AES密钥，然后发送方和接收方用AES密钥来通信。

#### [RSA非对称加密](RSA/)



#### [25519椭圆曲线算法](25519/)

Curve25519/Ed25519/X25519是著名密码学家Daniel J. Bernstein 在2006年独立设计的椭圆曲线加密 /签名 /密钥交换算法，和现有的任何椭圆曲线算法都完全独立，其中Ed25519用于签名

25519 系列曲线是目前最快的椭圆曲线加密算法，性能远远超过 NIST 系列，而且具有比 P-256 更高的安全性

OpenSSH 都迅速增加了对 25519 系列的支持，如今 25519 已经是大势所趋


### 为锻造最美之器

[![sites](qitas/qitas.png)](http://www.qitas.cn)
