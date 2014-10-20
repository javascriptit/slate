---
title: API Reference

language_tabs:
  - shell
  - python

toc_footers:
  - <a href='http://gitub.com/pycoin/pycoin'>pycoin on GitHub</a>
  - <a href='http://gitub.com/pycoin/pycoinnet'>pycoinnet on GitHub</a>

search: true
---

# Python Crypto-currency libraries

Welcome to the pycoin project, which consists of [pycoin](http://gitub.com/pycoin/pycoin) and [pycoinnet](http://gitub.com/pycoin/pycoinnet)

### pycoin
pycoin is an implementation of a bunch of utility routines that may be useful when dealing with bitcoin and some alt-coins. It has been tested with Python 2.7, 3.3 and 3.4.

```shell
pip install -e git+https://github.com/richardkiss/pycoin.git@2dcfaf5a4679f580fecb9ac72d33f40b4b066549#egg=pycoin-master
```

### pycoin net
pycoinnet is designed for use in conjunction with the Python pycoin library. It provides utilities and examples for writing tools in pure Python that speak the bitcoin protocol on the bitcoin network.

Note that is uses the new asyncio library included in Python 3.4 (and available from pypi in Python 3.3 -- type "pip install asyncio"), and so requires Python 3.3 or higher (unlike pycoin, which supports Python 2.7).
See also http://github.com/richardkiss/pycoinnet/ for a library that speaks the bitcoin protocol.

```shell
git clone https://github.com/pycoin/pycoinnet.git
cd pycoinnet
pip install -r requirements.txt
```

### Authors
pycoin is project of [Richard Kiss](https://github.com/richardkiss). Contributions and pull requests are welcome.

Want to donate? Feel free. Send to 1KissFDVu2wAYWPRm4UGh5ZCDU9sE9an8T. For bitcoin consulting contact: him@richardkiss.com.

# pycoin

## ku (Key Utility)
> ku is a command line utility (install pycoin through pip)

For responses in JSON format, simply use the -j option

### create

```python
# ku is a command line utility, the equivalent python code is:
```

```shell
ku create -j
```
> The above command returns JSON structured like this:

```json
{
   "BTC_address": "18TeXQN4y4kerR7h1xvaRUoMH5XXNeeupa", 
   "BTC_address_uncompressed": "14abkDyd4uA87aHdkaM1VcvmFAMQdZsXPD", 
   "address": "18TeXQN4y4kerR7h1xvaRUoMH5XXNeeupa", 
   "address_uncompressed": "14abkDyd4uA87aHdkaM1VcvmFAMQdZsXPD", 
   "chain_code": "a9a107c90c10a4d342988343c2e4d5e2e05418824e0bad48b64605fe50e0f4f0", 
   "child_index": "0", 
   "fingerprint": "51d304e4", 
   "hash160": "51d304e427c460beeda519d331769e964bf62bee", 
   "hash160_uncompressed": "27431ba2d49d514062fe38e704aec9cd5487bbe1", 
   "input": "create", 
   "key_pair_as_sec": "03aab2b7135822248dd66733530d9eb73fe3278db63e2be794d5aee8cd1af15485", 
   "key_pair_as_sec_uncompressed": "04aab2b7135822248dd66733530d9eb73fe3278db63e2be794d5aee8cd1af1548579d4d683d6b913f3667358b97e2601b1c5be7d19c8494d04241756d3401ea34d", 
   "netcode": "BTC", 
   "network": "Bitcoin mainnet", 
   "parent_fingerprint": "00000000", 
   "private_key": "yes", 
   "public_pair_x": "77208946577787814978834540915124044401684778022668014026381541902701082793093", 
   "public_pair_x_hex": "aab2b7135822248dd66733530d9eb73fe3278db63e2be794d5aee8cd1af15485", 
   "public_pair_y": "55105906784392444110946193675086405815876058795470459131838740250197852332877", 
   "public_pair_y_hex": "79d4d683d6b913f3667358b97e2601b1c5be7d19c8494d04241756d3401ea34d", 
   "public_version": "xpub661MyMwAqRbcGEPNJ3vKBVs5Vb9oKknjUrLXn6GZueAYW8ehxhEwE7fwYXGMUfAQRJCRiGS3iviWVnvBbKnTZCg6fenhoH7yLykgCXBT6YB", 
   "secret_exponent": "21736768208848952485277490635272827678808633926621495752266478612806703697575", 
   "secret_exponent_hex": "300e93275d00cb8ef686c43abf194643b6cbee48f4c5e1004d8e5d80536ecea7", 
   "tree_depth": "0", 
   "wallet_key": "xprv9s21ZrQH143K3kJuC2PJpMvLwZKJvJ4t7dQvyhrxMJdZdLKZR9vggKMThDMq9wrZcjoZctKjM34Ybq4RTb8iRPKeQGpsFWn2FiehnB7TfG6", 
   "wif": "Kxq8LRKNqod9xnidoR16T5tdR4xNNMLc63EUg8rWk89SdU3f8VzG", 
   "wif_uncompressed": "5JBT8a9hHwyDuWqraAyD7N3doEaqo59ySA7gMCJ7HZtJb6p5zwj", 
   "y_parity": "odd"
}
```

Create a BIP32 Key

`Entropy will be pulled from GPG and /dev/random`


## tx (Transaction Utility)

# pycoin net

## installation

