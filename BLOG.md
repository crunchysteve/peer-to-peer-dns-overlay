# WHY - WHERE - HOW - WHAT - WHEN
#### Short articles on making P2P as accessible as web 1 was.

<hr />

## 2024-02-26_1339 - Demonstrating the Vision a Little Clearer with a Picture

I've added a mockup screenshot of the idea of a non-registrant Peer-To-Peer, Personal Domain Name System to the whitepaper. It's an 
idealisation of the hard work that simple ideas often require, but a picture is worth 1111101000 words. &smile;
![whatTheWorldCouldLookLike](https://github.com/crunchysteve/peer-to-peer-dns-overlay/assets/46626696/c36357ad-0033-448d-8ee8-f42bd38c7129)

I dream of it being compatible with all the socket level hashtable protocols, be they torrents or ipfs, kademlia or chord. I suspect the best 
place to start for the network infrastructure would be with libp2p, as this is available in a range of programming languages, but notably 
C/C++. The idea would be to create the necessary hooks into the dht to present a dns entry attached to a given user's hash. Thus, the first
connection to a new contact, via their personal domain name, might take some time, even until their next time on the network, but once a
connection is made, that connection is cached at each end and connections will be as quick as any client/sever connection after that.

If you have any ideas for the more nuts and bolts of this, open an issue to ask to join the project and we can discuss your proposal. This 
will always be a FOSS project while I remain maintainer so, if that appeals to you, throw your ideas in the ring. We can discuss specifics in 
more private channels, if you wish, but start with generalities with an issue. I see my role as a "producer", such as in the context of radio 
production - an "art director" if film analogies make more sense to you. I can organise, moderate and inspire. I am also humble enough to
stand aside if somebody better suited to the task comes along. (For example, better understanding of the actual code than me.)

Cheers,
"Crunchy"

<hr />

## 2024-01-23_1339 - Oh, And One More Thing

This blog, being part of a repo, can be forked, that fork editted, then pull-requested back. If I like your contribution...

Pull approved! So, even if you can't code at the system level, hell, I'm an Arduino hack, I can't code much beyond making clicks and bleeps 
come out of a 328p chip, you can still contribute conceptually, Like I'm attempting to here. This idea is a democratic approach, aiming to 
make potential/future users part of the design team. Code will only be accepted under an MIT licence. This is how I want to make the world 
a better and much safer place. Leave the world better than you found it when you go is my goal.

<hr />

## 2024-01-23_1246 - Too Many Platforms, No Real Solutions

I2P is not really operable with IPFS. IPFS isn't as operable with the conventional network as the hype suggests. Just like domain names are 
easier to remember than IP numbers, this idea I'm proposing, an offline-first, distrubuted DNS, capable of hosting any, random domain name 
as a human-readable handle that *points to* the underlying secure userhash, the unique gibberish, as I like to call it.

The internet existed for quite a while before the "World Wide Web" came into being. It was an academic tinkertoy. A nerd tool, a boffin's 
link. What opened it up to us was the human readability of me@mymailbox.com and www.myblog.net and decentralisation expects us to read...

```khjgasdkhjfxggesfmBCSYSZRBEMFBAJDHBSGHFDAKJHDGhgfjskhabdfkagh```

Yes, I just clattered my keys randomly and, even the most autistic among us could not remember that hash if I deleted it, or any hash generated 
cryptographically, for that matter. Now, as I say in my [whitepaper](./README.md), if we choose random words, just from English for now, but 
nearly any other language, We get immeasurable possible human readable "word salads" to use for random ID. Bring in all the languages, we get 
even more diversity that is low-to-no-conflict by design. Even allowing the option of choosing your own word salad, or appending your own name, 
handle or real name to the left as a subdomain reduces, rather than increases the risk of domain name conflict. No registration required.

In this environment, there are no servers, not clients, no domain registrars or registrants, the Personal DNS System can be as simple as a 
graph database. So, because this idea completely revereses the whole, top-down heirachy, to a user-up model, I like to refere to it as PDNS,
and to any individual's choice of domain name string, their PDN. Political anarchists should see an immediate benefit to this system, that it 
is community owned and driven. In fact, really, only the greedy and self-interested could see harm in this type of peer-to-peer network 
addressing protocol. It's a concept that can be as free as beer, let alone as free as speech.

There are tools already in existance that are useful to this model. BIND should work with any domain name system, it just needs a fork and a 
patch. Gun.js is an example of a database tool that is ofline-first and distributed. It's javascript, so maybe it's not the guts of a network
infrastructure, but a quick google reveals other graphDBs in more systems design grade languages. I'm not talking about peer-to-peer being an
applications layer, I'm talking about it being network systemic - using UDP and/or TCP/IP at the network level, as an infrastructure protocol. 
Still back-compatible, sure, but every device becomes its own server, and every peer can request anything from any peer it has the public key 
for and user permissions to access. Any user can also find their new friend or colleague by a handle that looks like...

```pttps://crunchysteve.randomly.chosen.human.words.here``` or ```pttps://crunchysteve.actually.chose.this.handle```

This model has more permutations per person than there are lightyears to the centre of the universe. Way more! This model expands to absurd 
levels of permutation if we include all the wiktionary languages. Yet, protocol's the interface apps' databases will never need to hold more 
than that app's user's friends PDNs and will only need to sync and conflict resolve the occasional new connection or resolve the odd conflict. 
Conflict resolution is even soluble by a user adding one word to their PDN, or possibly removing one. Random might be the default, but user 
choice should be there, too.

It's a bottomless, self-managing labelling database. And like DNS hides our IP numbers, this hides our public hashes, makes them a key on our 
keyring, rather than using our lock as our street address, which current hashtable peer networks do. It's actually more secure.
