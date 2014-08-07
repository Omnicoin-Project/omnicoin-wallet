Welcome to _Omnicoin Wallet_, a standalone omnicoin payment app for your Android device!

Omnicoin is an experiment in the creation, implementation, and integration of a cryptocurrency with MyBB community software in mind. 
Originally created by a member of HackForums.net it's grown beyond that initial ideal and has moved into a wider realm of possibility. 
With a new launch of version 2 (OMCv2), a new team, and renewed focus Omnicoin promises to gain ground which no other crypto currency has tread.

![alt tag](https://encrypted-tbn3.gstatic.com/images?q=tbn:ANd9GcT5cGH94w6MbLPaBojOdBAVmPM9pbqJm3LIn2gNd4tPKd1F8qbgmg)

This project contains several sub-projects:

 * __wallet__:
     The Android app itself. This is probably what you're searching for.
 * __market__:
     App description and promo material for the Google Play app store.
 * __integration-android__:
     A tiny library for integrating omnicoin payments into your own Android app
     (e.g. donations, in-app purchases).
 * __sample-integration-android__:
     A minimal example app to demonstrate integration of omnicoin payments into
     your Android app.

You can build all sub-projects at once using Maven:

`mvn clean install`
