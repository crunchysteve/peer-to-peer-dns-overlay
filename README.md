# A Whitepaper Proposing Peer To Peer Hashtables Having a DNS Overlay

A whitepaper to propose a human readable p2pDNS layer over a peer-to-peer hashtable, to jump past web 3 directly to web 4, using the oldest idea 
on the internet, DNS.

## Premise
The idea is to seed the concept of a "Personal Domain Name" and, generally personal DNS (PDNS), into the developer community, with the view to 
there being a human-readable layer over existing user-chosen, peer-to-peer hashtables, effectively hiding the hashtable from view, much like DNS 
hides our IP4 and IP6 network addresses behind registered domain names.

Such PDNS names might consist of a profile handle (in my case, crunchysteve, for example) and 3 to 6 words of 3 to 6 characters length, chosen at 
random from wiktionary (for example), such that my Personal Domain Name (PDN) might be generated randomly by such an app as, 

```crunchysteve.pluck.city.horse.fiddle```

Initiating a social conection to me on such a PDN might be via,

```pttps://crunchysteve.pluck.city.horse.fiddle```

Or, I might ask this app to verify no conflict or preexistance regarding a chosen domain like,

```crunchysteve.amateur.engineer.and.guitar.player```

From this chosen domain, it would send out a search for potential conflict over the DHT. Considering it contains my handle, as well,
conflict is unlikely to occur.

By using a dictionary lookup for selecting random words, based on choosing 3 to six, 3 letter to 6 letter words, probably leaves 500,000 possible
words from wiktionary's more than 700,000 english words. This gives 500,000 to the 3rd power plus 500,000 to the 4th power plus 500,000 to the 
5th power plus 500,000 to the 6th power PDN combinations, or 1.25 x 10^17 + 6.25 x 10^22 + 3.125 x 10^28 + 1.5625 x 10^34 which is greater than 
1.562503125006 x 10^34 possibilities. 1.929 x 10^24 possible domain names for every human on the planet. With this hiding a 128, 256, whatever 
higher bit count hashtable makes uniquness and security built-in while simplifying accessibility for communicating addresses to others. The PDN
becomes the address, the hash becomes the key to the locked door. How humans actually work and live, overlaps no longer become a problem, just
a brief glitch as the system offers an alternative, should it have detected a conflict.

## Aims
The aim of this whitepaper is to 
 - inspire the development of the necessary protocols and overlays to hide complexx peer-to-peer hash addresses from
the end user, making peer-to-peer networks more accessible and as easy to use as web1 was.
 - create a relatively malleable model for creation and conflict resolution for PDNs and the PDNS that allows forms like,
   - using a PDN with or without a user handle as a subdomain (eg word.people.bag.puddle or fred.word.people.bag.puddle)
   - shared peer clusters (eg me.word.people.bag.puddle and you.word.people.bag.puddle)
   - conventional DNS overlays (eg connections to example.com display the standard domain but are connected to a PDNS)
   - resolve conflict by prior ownership or agreed transfer of prior ownership to new owner
 - achieve a protocol that can be recognised by the IETF as the network standard for hashtable peer-to-peer networks,
 - prevent proliferation of incompatible, "upper-layer" models for peer-to-peer networking.
 - make data harvesting centralised systems less operable or even inoperable.
 - make peer to peer connection human readable, memorable and fun, as a layer on top of hashtable security

The idea is not to eliminate client/server for such things as it is necessary, such as for business identity, government services, etc, rather it
is to provide an accessbile, "non-nerd" addressing system for the secure interconnection of individuals, groups, group-to-individual and 
individual-to-group interactions.

## About the Author, Crunchysteve
I have grander ideas than my skills but a white-hot focus on the principles of those structures, as well as being a reader of the technical 
principals behind my ideas. Being only an Arduino hobyist, I know only some basic C/C++ but am embarked on learning it more formally, if
self-paced, but I also have 27 years experience with the internet, generally. I have run servers, managed media storage/retrieval systems and
understand the principles of DNS to a small system manager level. I have a passionate commitment to internet decentralisation and security, I
oppose the current tendency of the world towards digital feudalism and I'm no "blockchain bro." I'm 62, retired from a 3 decade career as an
audio producer in radio and know how to organise a small project. Feel free, if inspired, to pull request your code ideas, or mods to this
whitepaper.
