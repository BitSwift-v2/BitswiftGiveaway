# BitswiftGiveaway
 Bitswift Tablet Giveaway
 
 This source code was used to determine the winner of the Bitswift Tablet Giveaway.
 
 The SHA-256 HASH of this .TAR file, 
"0c42b13496380876da25e83f66b9d79e38ffc57ac3586bb9cc77416b86728afc"
 was injected into the Bitswift Blockchain within transaction ID:
 4:4241eba0807c8bdcfd6ff9e48704e02b683590416cec65712a744704d4533c50
 
 The app was then later run using the below secretforRandom which determined a random winner.  
 
To run the application extract the contents of a tar file onto your computer running a local Ardor server.
Edit the configuration.json file to meet your particular application requirements. 

 An sample of the configuration.json file is below:

{
  "contractName": "BitswiftGiveAway", //this can be anything you want to call the contract 

  "secretForRandom": "4eca220d667c151c66f3abf0d1f9b7829e4627558dacaec56e0a07f4b3e5cf32", //64 bit random hex string used to determine a random winner

  "useLowSecurityRandom": false,
  "isVerifier": true,
  "verifyAccount": "15925665273593510758",

  "messageForPick" : "MicrosoftSurfaceTablet", //The specific message the application will look for

  "heightStart": 2027000, //Application will start at this block height
  "heightStop": 2132393, //Application will stop at this block height

  "transactionChain": 4, //Specify the chain the application is running on

  "stateRootDirectory": "state",
  "reloadAndRescan" : false,

  "api": {
    "password": "xxx", //the api password of your blockchain node set in your nxt.properties file
    "host": "localhost",
    "port": "40004"
  },

  "protocol": "http",
  "host": "localhost",
  "port": "27876"
}

