# FakeBlock

FakeBlock a social network for the rest of us. Inspired by George-Micheal Bluth's product of the same name, FakeBlock aims to be an ad-free, decentralized, prviate, secure, open-source socail network. This is not an app for connecting with elementary school friends. It's an app for building and maintaining real connections.

## Connections

Unlike other social networks, FakeBlock's social core resolves around the idea of building 'connections' with others. NOT friends. In the social networks of today, the concept of a friend has been gutted and turned into a marketing tool and a sign of social status. Connections, as a concept is something bigger. Connections are varied, they can change and they can attrophy. 

### Types of Connections

*Note - More types of connections can be added but the word 'friend' is not allowed. Connections are defined as a relationship between two people that is eternal. For instance, no matter what happens a Child will always be a Child to a Parent. Connections are also topical as in the relate to something both locally shared by both users.

- Parent
- Grandparent
- Child
- Sibling
- Spouse
- Relative
- Colleague
- Teammate
- Classmate

#### Creating Connections

Users on FakeBlook create connections with other users via in person communication. In fact, a connection can not be created with another user unless that person is within a given proximity. After which, the users can continue to connect with each other over any distance. 

#### Connection Attrophy

Connections that are not maintained, as in the real world, will begin to attrophy. Once fully disconnected, users will need to re-establish them with end person contact. Connections are maintained and stregthened through simple, basic communication. The more communication, the better the connection will be. 

## Features and Goals

### Primary Features

- Messaging
- Calling
- Photo and content sharing

### Goals

**Secure**
- Security first
    - open source
    - encrypted everything: mesaging, calling, photos sharing
- Secure encrypted messaging
- Secure encrypted calling
- Secure encrypted photo and media sharing
- Password-less: All authentications performed bia on-device security and public key chains of trust. 

**Authentic**: 
- All interactions are initiated via in-person contact mean that two users *must* know each other in real life. This helps ensure that who you think you're talking to is actually who you're talking to. 
- The lack of having connections rather than 'friends' means you never have to worry about unfriending someone who you know longer care to be associated with. Connection links will organically grow and dissolve as they do in the real world. 

**Trusted**
- Private and ad free. None of your personal data ever leaves your device and data stored in the cloud is encyrpted using a key that only you have access to. 
- Free: A free teir will exist which is subsidized by those paying for more connections. 
- Local: In the event you want to run you're own server and create your own network, that's okay too. 
- Labeled: All data shared in public will be scrutized and labeled for credibility. 
- Users will be unable to share data which contains information about others without the permission of those individuals. 

- The components

### Handshake

- Two devices verify each other using both proximity and shared keys. Bluetooth for proximity and scanning of QR codes to exchanges keys

### User validation

- A user can be validated by having their public key signed with a by a key from another user who has also been verified. 
- Verification involves a chain of trust. This present an interesting problem of scale. How can you have a chain of trust spanning hundreds or thousands of certificates

## Components

- **FakeBlockCore**: Core libraries, Messaging, Photos, Video, Audio, User Relational Components
- **FakeBlockAndriod**: Android app
- **FakeBlockiOS**: iOS app
- **FakeBlockWin**: Win app
- **FakeBlockMac**: Mac app
- **FakeBlockNix**: Linux app

## Chain of Trust

1. root key
    - subroot 1
        - user key
            - user key
                - user key
            - user key
                - etc...
        - user key
    - subroot 2
        - user key
        - etc..
    - subroot 3
        - user key
        - etc...

**Workflow**

- A root key is created
- The root key signs 3 admin keys. Admin keys are special keys that do not need to be verified and function as proxy for the root key. They are essentially intermediate CAs. Once signed, the 3 admin keys are instantly set as verified users. This allows them to sign any number of user keys.  
- The admin keys begin signing users keys. 
- A user key must be signed by 3 other verified keys to become verified. Once verified, a user key can begin verifying other user keys by signing them.
- Eventually all users on the platform will become verified users. 

**Result**
- Verified users on the platform will have special benefits and can also restore their accounts from encrypted server side backups. 
- On each user's device will contain their encrypted private key
- Essentially, every user then has a key that has been signed and contains a valid chain of trust to trace back who they are. 

( I'm sure there's a good mathematical formula for this...still working it out. )