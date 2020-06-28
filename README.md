# ShitCoinMoloch
Stable Moloch for ShitCoinDAO

## Moloch V2 Designed w/ ShitCoin DAO Requirements in mind. 
Built with the following extensions to the standard moloch: 

## Magical Minion 
Summon a MinionSummoner first and then attach to your Moloch Summoner. This will create a minion for each Moloch without having to do any extra work. 

## Summoner Circle 
Add multiple summoners to your DAO. Works basically the same as adding multiple approved tokens at the time of summoning. Each summoner will be admitted as a member and issued a single share. 

We also added a makeSummonerTribute function that allows these summoners to add tribute at a pre-defined rate of or tribute to shares via setting the summoningRate, which will be the denomator in determing shares (i.e. shares = (tribute / summoningRate)-1. The 1 share is deducted so that summoners don't get an extra freebie share if they take advantage of this function. The rights of summoners to use this function is also time-limited by the summoningTime, which is set in the constructor. 

*Adding too many summoners could result in a function that exceeds gas limits, but you can also always add people through the proposal process. 
