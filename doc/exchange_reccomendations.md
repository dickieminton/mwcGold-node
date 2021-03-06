<p>There are some important things to note about exchange support for MWC. As with all POW blockchains, reorgs and double spend attacks are possible. With Mimblewimble, it is harder to detect the attacks because there are no addresses and only outputs. The network is young and reorgs have happened in our early history.
<p>
<p>The current mwc-wallet (2.4.6) has a check feature that can help detect double spends or coins that no longer appear after a long reorg, but it is based on the grin 2.0 wallet and has some bugs. The most reliable way to detect double spends is do a recovery from seed.
<p>
<p>In master of our github, we have the rebased 3.0 wallet from grin and will be releaseing it shortly. We also have made several fixes on top of the grin wallet which to fix additional bugs related to double spends and reorgs. We are still testing these features, but will release the mwc-wallet soon. It can be built from master and used for testing now.
<p>
<p>Reorgs are getting harder to do, but we still recommend a high number of confirmations to ensure funds are secured. One way to ensure funds are actually available is to require a particular amount of confirmations and then regularly sweep all the funds in the recieving wallet to either cold storage or another withdrawal wallet. This is a standard architecture for exchanges and may prevent losses from double spend or reorg attacks.
