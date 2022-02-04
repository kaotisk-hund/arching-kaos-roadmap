# Arching Kaos Transition Roadmap

> Version 1 -> Version 2

## General outline
Below you can see a table with some basic utilities that arching-kaos as a project serves currently in version 1. Version 2 is under development.

| Utility | V 1 | V 2 |
|---|---|---|
| instant messaging | irc + matrix | *tba* |
| webpages | nginx + fs + sql + ipfs | *tba* |
| webradio | ak-api + ipfs + liquidsoap + icecast + webpage + ssb | mixtapes + ak-dr |
| donations | btc | xlm |
| payments | n/a | ARCHINGKAOS + KAOTISKHUND |
| support | trac | *tba* |
| news | git | news |
| blog | wordpress/docsify | *tba* |
| profile | multiple based on network (e.g. ssb) | profile |

## Completion stages

- [ ] - instant messaging
- [ ] - webpages
- [ ] - webradio 
  - [ ] - ak-api -> mixtapes
  - [ ] - liquidsoap + icecast -> ak-dr
  - [ ] - ssb -> ?
- [x] - donations
- [x] - payments
- [ ] - support
  - [ ] - tickets 
  - [ ] - components 
  - [ ] - milestones 
- [x] - news
- [ ] - blog
- [x] - profile



## Explaining utilities and plans

### Webpages
Pages for now across arching-kaos project are mostly static. From the land of the [portal](https://arching-kaos.net) to the [index](https://arching-kaos.com), mostly static layouts with some fluidity in their content. Most of pages are "packed" into a single html file where everything takes place.

A member of the community can of course have a webpage. #TODO This will take more writting

### Webradio
Please see https://github.com/kaotisk-hund/arching-kaos-decentralized-radio .

### Donations
Donations were accepted in BTC. However, BTC is not our best option mainly of its price and fees. Since arching-kaos supports assets on Stellar network a donation address will be available to drop some XLM, KAOTISKHUND or ARCHINGKAOS. The donations are going to be distributed to the expenses of the project as well as pay some percentage of the amount to the developer (me for now) for every commit to the project.

### Payments
Payments were not possibles in version 1. Now, there are two assets (ARCHINGKAOS and KAOTISKHUND) that can someone use to make payments to anyone they want.

### Support
For support purposes, apart from other forms of communication a _centralized_ support system is in use. Trac. Trac is an awesome tool for project management. Using it, it is fun and features that come with it make it very handy for managing projects. I had developed MPPM (my personal project manager) in PHP for the same reason and also by admiration to Trac's everything. Of course this didn't go that far.

Note that I mostly focus on 3 sections of trac:
1. tickets
2. milestones
3. components with versioning 

- So how about a decentralized edition?
- Of course!

We will be having fun!

- [ ] - tickets (add/reply/etc/close/reopen)
- [ ] - milestones (create/add-ticket)
- [ ] - components (add/edit/remove)



### News
Experimenting with ways to share the news of the project, I used SSB mainly but after a while I got into sharing via other means as well.

To evolve this from protocol specific feed, I switched to a simple git repository hosted on a cgit (interface) instance.

Nice style, but yet...

- [x] - news

Arching Kaos Tools comes with the `news` command.

### Blog
Wordpress is a content manager. The b in blog I don't understand. It's a log. Whatever. Other methods? Yeah, I write the content in markdown and use docsify to render it  nicely. Other? Of course, see above. Consider it duplicate?

### Profile
> Profile? Well in IRC you can find me as ... and in matrix as ... and my email is ... and ...

So we got no profile for version 1 but we get our profile in our configuration of our address and (of course) on our personal infochain.

### Instant messaging
IRC and Matrix are both distributed and decentralized networks already. However, what happens if the servers grow in visits?
People then could assist on expanding the networks. Offer IRC linking or whatever.

For v1.0 I tried to work on a auto-peering script for IRC. For this, you need to be able to modify the configuration file every time someone is "registering" to the network. Mainly, with CJDNS someone could use `python-cjdns-peering-tools` to connect with the public servers and furtherly for their established connections (cjdns wise) try to connect IRC using CJDNS IP for connecting and public key for credentials ("secret").

To my ears, it sounds both amazing and sloppy. Also, matrix could require further contact etc.

So to go to the second version, a chat system should be created.


