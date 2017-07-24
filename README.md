# snatcoinVanity


The current reccomended method for generating a SnatCoin Vanity Address is to use samr7's BitCoin vanitygen, which is avaliable at https://github.com/samr7/vanitygen

For some more information on how to use this tool, please visit https://github.com/snatcoinOfficial/snatcoinVanity/wiki/Using-samr7's-vanitygen

Once you have generated a vanity address to your likely using their tool, go to the SnatCoin website, free F12 to open the developer tools, enter the following, remembering to replace where it says "PRIVKEY FROM VANITY gen" with the Private key generated by the vanitygen tool.

This will return a usable SnatCoin Private key, matching the vanity public address.

Bitcoin.Base58.decode("PRIVKEY FROM VANITY gen").map(x=>{var p=x.toString(16);return(p.length>1?"":"0")+p;}).slice(1, 33).join("")


If anyone wants to make this easier for the end user feel free to do so :)
