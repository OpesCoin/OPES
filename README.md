OPES integration/staging tree
================================  
What is OPES? 
----------------
  
OPES is the cryptocurrency.  

  
### Specification 
 - Scrypt-salsa64+Argon2 PoW algorithm 
 - 60 seconds block targets 
 - 52000000 total coins 
 - 20 coins per generated block 
 - Subsidy is reduced by 5% every 86400 blocks, which will occur approximately every 60 days
 - DGW_v3 difficulty regulation 

### Ports 
 - RPC 6223
 - P2P 6222
 
### Compilation issues
 
#####Error

	$ undefined reference to `leveldb::Status::ToString() const


#####Solution

	$ cd leveldb
	$ chmod 755 build_detect_platform
	$ make libleveldb.a libmemenv.a
	$ make clean -f makefile.unix
	$ make -f makefile.unix 



License 
-------

OPES is released under the terms of the MIT license.  
See http://opensource.org/licenses/MIT for more information.  

Copyright (c) 2009-2014 The Bitcoin developers  
Copyright (c) 2013 The Blakecoin developers  
Copyright (c) 2013 The Litecoin developers  
Copyright (c) 2014 Fuguecoin developers  
Copyright (c) 2014 GroestlCoin developers  
Copyright (c) 2015 The OPES developers  
