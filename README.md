# Kaggle Project. Facebook Recruiting IV: Human or Robot?
Predict if an online bid is made by a machine or a human

## Data
### Description
There are two datasets in this competition. One is a bidder dataset that includes a list of bidder information, including their id, payment account, and address. The other is a bid dataset that includes 7.6 million bids on different auctions. The bids in this dataset are all made by mobile devices.

The online auction platform has a fixed increment of dollar amount for each bid, so it doesn't include an amount for each bid. You are welcome to learn the bidding behavior from the time of the bids, the auction, or the device. 

The data in this competition comes from an online platform, not from Facebook.

### Files

* train.csv - the training set from the bidder dataset
* test.csv - the test set from the bidder dataset
* sampleSubmission.csv - a sample submission file in the correct format
* bids.csv - the bid dataset

### Data fields

#### [ the bidder dataset ]
* bidder_id – Unique identifier of a bidder.
* payment_account – Payment account associated with a bidder. These are obfuscated to protect privacy. 
* address – Mailing address of a bidder. These are obfuscated to protect privacy. 
* outcome – Label of a bidder indicating whether or not it is a robot. Value 1.0 indicates a robot, where value 0.0 indicates human. The outcome was half hand labeled, half stats-based. There are two types of "bots" with different levels of proof:
  1. Bidders who are identified as bots/fraudulent with clear proof. Their accounts were banned by the auction site.
  2. Bidder who may have just started their business/clicks or their stats exceed from system wide average. There are no clear proof that they are bots. 

#### [ the bid dataset ]
* bid_id - unique id for this bid
* bidder_id – Unique identifier of a bidder (same as the bidder_id used in train.csv and test.csv)
* auction – Unique identifier of an auction
* merchandise –  The category of the auction site campaign, which means the bidder might come to this site by way of searching for "home goods" but ended up bidding for "sporting goods" - and that leads to this field being "home goods". This categorical field could be a search term, or online advertisement. 
* device – Phone model of a visitor
* time - Time that the bid is made (transformed to protect privacy).
* country - The country that the IP belongs to
* ip – IP address of a bidder (obfuscated to protect privacy).
* url - url where the bidder was referred from (obfuscated to protect privacy). 

details: https://www.kaggle.com/c/facebook-recruiting-iv-human-or-bot
