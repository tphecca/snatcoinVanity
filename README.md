# snatcoinVanity


use addrgen.py which is from https://github.com/weex/addrgen/blob/master/addrgen.py originally



To Use

Bitcoin.Base58.decode("PRIVKEY FROM VANITY gen").map(x=>{var p=x.toString(16);return(p.length>1?"":"0")+p;}).slice(1, 33).join("")


If anyone wants to make this easier for the end user feel free to do so :)
