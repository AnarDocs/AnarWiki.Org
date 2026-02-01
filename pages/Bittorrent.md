'''What follows are instructions for setting up a good, secure
[Bittorrent](http://en.wikipedia.org/wiki/Bittorrent) client
([Deluge](http://deluge-torrent.org)). Bittorrent may be used to
download anything, just like HTTP. That means content that's legal to
download, illegal to download, and ambiguous under laws like the DMCA.

These instructions may be selfish or greedy (i.e. not sharing much) but
are a good solution for the (justifiably?) paranoid. Sharing is caring,
however, and you may want to consider more generous settings.'''

# The Protocol

Bittorrent is a protocol, so you need to think of it as a thing that's
not tied to a specific program (a "client"), just like the protocol HTTP
(the Web) is not tied to a specific client (you can use any browser like
Firefox, Internet Explorer, etc.)

There are a lot of bittorrent clients. There is even a client called
BitTorrent, confusingly enough, but don't conflate the **method of file
transfer** with the **software negotiating that transfer**.

# Deluge Client

Deluge is simple, doesn't suck up too much RAM, and offers a fair amount
of protection from surveillance (random ports, encryption, a blocklist
plugin). It runs on Windows, Mac OSX, and GNU/Linux. Another simple
alternative is [Transmission](http://www.transmissionbt.com).

- Go here, download the installer, and run it:

<http://deluge-torrent.org>

After you've installed Deluge (and the GTK+ runtime that's bundled with
it), take a look at the screenshots below. These are from **Edit \>
Preferences**, and they may be slightly different from what you'll see
on your machine. Go through each and try to copy the settings.

## Screenshots

<figure>
<img src="Deluge01.png" title="Deluge01.png" />
<figcaption>Deluge01.png</figcaption>
</figure>

<figure>
<img src="Deluge02.png" title="Deluge02.png" />
<figcaption>Deluge02.png</figcaption>
</figure>

<figure>
<img src="Deluge03.png" title="Deluge03.png" />
<figcaption>Deluge03.png</figcaption>
</figure>

<figure>
<img src="Deluge04.png" title="Deluge04.png" />
<figcaption>Deluge04.png</figcaption>
</figure>

<figure>
<img src="Deluge05.png" title="Deluge05.png" />
<figcaption>Deluge05.png</figcaption>
</figure>

<figure>
<img src="Deluge06.png" title="Deluge06.png" />
<figcaption>Deluge06.png</figcaption>
</figure>

<figure>
<img src="Deluge07.png" title="Deluge07.png" />
<figcaption>Deluge07.png</figcaption>
</figure>

### Notes About Blocklists

- Blocklists are not perfect, and change often or may stagnate for
  (seemingly) no reason. Also, they may be infiltrated by malicious
  users. For a frequently-updated list of blocklists, see
  <https://sites.google.com/site/blocklist/>
- The safest blocklist to use is probably the SafePeer "Paranoid" list:
  <http://www.bluetack.co.uk/config/psplist.zip> or
  <http://blocklist.googlepages.com/psplist.zip>
- Make sure you check the blocklist URL in Deluge's plugin settings
  often.
  - You probably won't need it if you have Deluge's blocklist plugin
    installed and are using a current blocklist, but there are also
    programs specifically designed to
    "<a   href="Bittorrent#Bad_Peers.md" class="wikilink"
    title="block bad peers">"block bad peers</a>.

# Getting Files

Now that you're done with that, it helps to understand a little more
about how bittorrent works. Basically, you go out on the Web or request
a "tracker" from someone directly. In almost all cases, this will mean
going out to a popular bittorrent website and downloading a tracker file
(.torrent), which you then open up in Deluge...the first time you do
this, you'll want to tell your browser to try to do it automatically.

After Deluge reads the tracker file, you can delete it (it's just a text
file with instructions for Deluge or any other client). Now, Deluge will
try to download pieces of the file from as many users as possible, while
also sharing some of those pieces to other people as you get them. The
beauty of this is that you can download from people who are sharing the
whole file ("seeders") while you also grab from people like you who
don't have the whole thing yet ("leechers"). If there were no seeders
for the file, then you would never get the whole thing.

## Popular Sites

For many users, the next step is to go out to
[PirateBay](http://en.wikipedia.org/wiki/Piratebay) (NSFW) and search
for something popular. Although we don't recommend these sites, you
should protect yourself if you do decide to use them. You'll see a bunch
of things on the search results page, including porn ads if you don't
use an adblocker (like [Adblock
Edge](https://addons.mozilla.org/en-US/firefox/addon/adblock-edge/) for
Firefox).

Here is a [list of sites that link to free and legal
torrents](http://gigaom.com/2007/03/03/ten-sites-for-free-and-legal-torrents/).
On any site with bittorrent links, you'll want to sort the results by
seeders (e.g. click the bolded "SE" on the right of the search results)
and then click the icon below the title of the torrent you want (this
icon is usually a magnet). Always look for as many seeders as possible,
unless you don't have a choice.

## Notes About Magnet Links

- Most bittorrent sites have switched to [magnet:
  links](http://en.wikipedia.org/wiki/Magnet_links) relatively recently
  (you'll usually see a magnet icon). If you're having trouble opening
  these links with Deluge, there are [a number of
  solutions](https://duckduckgo.com/?q=magnet+links+browser+help).

## Finished Downloads

The .torrent file will download and you need to open it with Deluge if
it doesn't happen automatically (depends on your Web browser). Then,
Deluge will do its thing and you just wait. After the file downloads, it
will try to seed the file (making you a "seeder"). After the file
downloads 100%, you can find it in that "finished" folder from the first
screenshot. In Deluge, you may want to right-click any seeding files and
choose "Remove Torrent". Don't accidently "Remove Torrent and Data" or
you can guess what will happen.

# Misc

- Files compressed as .rar are usually password-protected to force
  people to go to malicious websites, so you'll want to steer clear of
  them.
- To open other compressed files, you'll want to install
  [PeaZIP](http://peazip.sourceforge.net/) or see
  "<a   href="Libre_Recommendations#Utilities.md" class="wikilink"
  title="our list of alternatives">"our list of alternatives</a>.
- To view pretty much any multimedia file, you'll want to install [VLC
  Media Player](http://www.videolan.org/vlc/) or see
  "<a   href="Libre_Recommendations#Media_Players.md" class="wikilink"
  title="our list of alternatives">"our list of alternatives</a>.
- Clear as mud? It seems complicated, but sometimes it's better to
  overexplain than underexplain and you end up banging your head against
  a wall. After the first file you grab, you'll see it's not difficult.

## Bad Peers

- [PeerGuardian](http://sourceforge.net/projects/peerguardian/) and
  [PeerBlock](http://www.peerblock.com/) are firewalls to block known
  bad addresses from investigating you.
  - [More info
    here](http://netforbeginners.about.com/od/downloadingfiles/a/peerblock_p2p_anonymity.htm)
- [MoBlock](https://help.ubuntu.com/community/MoBlock) and
  [PGL](http://sourceforge.net/p/peerguardian/wiki/pgl-Main/) are
  alternatives for GNU/Linux.
- You probably won't need these if you have Deluge's blocklist plugin
  installed and are
  "<a   href="Bittorrent#Notes_About_Blocklists.md" class="wikilink"
  title="using a current blocklist">"using a current blocklist</a>. But,
  these programs will act as a firewall for any network connection, not
  just bittorrent.

# OneSwarm

- [OneSwarm](http://www.oneswarm.org/) is a file sharing program that
  utilizes
  "<a   href="Bittorrent.md" class="wikilink" title="Bittorrent">"Bittorrent</a>
  for strong anonymity. It a "[friend of a
  friend](http://en.wikipedia.org/wiki/FOAF_%28software%29)" model.
  - Check out this great paper by the devs, [Why My Printer Received a
    DMCA Takedown
    Notice](http://www.michaelpiatek.com//papers/piatek_hotsec08.pdf).