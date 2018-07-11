# FakeBlock - ( In Planning Phases )

FakeBlock, inspired by George-Micheal Bluth's product of the same name, aims to be a free, decentralized, open-source, social network for the rest of us. This is not an app for connecting with elementary school friends. It's an app for building real relationships. 

## Goals

- **Decentralized**: Using p2p technology FakeBlock will allow user data to be stored in a decentralized network of nodes that will run free from corporate and government influence to provide the greatest stablity. Small chuncks of the FakeBlock network will be distributed to all FakeBlock users who will then host them. 

- **Secure**: Using block chain technology FakeBlock will ensure that users data is crypotgraphically secure. To prevent from abuse, user will be validated based on their real world connections to other users. All logins are passwords less: Users are initially verified by other verified users who are on the site; Users log in using keys stored on their FakeBlock devices; If a device get's lost or replaced, a user can reregister a new device by verifying their identity with their originaly verified friends. 

- **Authentic**: From a social networking perspective, FakeBlock aims to be the most authentic by requiring that users who connect to each other through FakeBlock know each other in reality. The FakeBlock app uses NFC/BlueTooth to verify when you're in contact with another FakeBlock user. All logins are invite only, meaning you need to personally know another FakeBlock user to begin using the service. The less active your interactions with your FakeBlock friends the less you'll see them within your profile and eventually they'll disappear alltogether and you'll need to reconnect with them in real life to add them again. 

- **Trusted**: Users will be allowed to share lots of forms of content with their friends and the FakeBlock community but all content will be tagged and labeled using an automatic vetting process to allow users to make correct judgements as to the validatity of the statement. Using FakeChecker ( a component of FakeBlock ) a given claim will be checked for sources in a recursive fashion. The deeper the source links, and the more numerous credible sources that are found, the higher the score of the statement, and the higher the credibilty of the commentor. Each user can then decide based on the labels what to think the content being presented. 

## Build

This app is being built using Xamarine for both Android and iOS compatiblity. Web compatiblity will be next on the agenda. 

## Components

- **FakeBlockCore**: Core libraries including UI, Messaging, Photos, Video, Audio, User Relational Components
- **FakeChecker**: Libraries to scan a given statement and return a label with metadata about the validity of the statement. 
- **BlockSync**: Engine which descributes the FakeBlock core service amount various hosts. 
- **FakeChain**: Block chain backend storage mechanism for user data. 

## Open Source Components to Utilize

- SignalProtocol: Secure messaging
- ...

## Roadmap

- [x] - Create basic project plan and readme. 
- [ ] - Set up project development environment and push.
- [ ] - Create a proof of concept App UI
- [ ] - Create a proof of concept animation detailing various user interaction scenarios. 
- [ ] - Create a asymentric key based login mechanism using LetsEncrypt certificates. 
- [ ] - Create a bluetooth based user authentication and verification process for users who are in close proximity
- [ ] - Create a sql databsaed backed by a backend blockchain which is hosted on each users' device. 
- ..

## Technologies to Learn

- Blockchain building
- Crypotgraphy and public private key pairs
- C# ( Xamarin )
- Swift (iOS)
- Java ( Andriod )
- Javascript ( Web )
- ...

## Contribute

- I'm still in the planning phase but if you have ideas, questions or suggestions, just make an issue!

## Maintainers

- geogboe - George

## Copywrite

2018 - Present @Adeium.net
