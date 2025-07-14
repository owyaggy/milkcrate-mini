---
layout: page
title: Music Discovery
permalink: /discovery/
---

### How Does Music Discovery Work?

The site will focus on six major facets of modern music discovery:

1. Collaborative filtering
2. Content-based filtering
3. Playlistification
4. Modern payola
5. Bias toward popular music
6. Conversion to lean-back

### Collaborative Filtering

Collaborative filtering is a technique based on the premise that if someone is searching for new music, they would highly value recommendations from someone with whom they share many common musical interests.

In practice, this means that for a given user, a streaming service (e.g. Spotify) can identify a group of users with similar music taste, and reommend new music from those users to the current user.

At the scale of these platforms, these recommendations are the basis of millions of aggregated statistics, preventing any meaningful transparency. It's not the case that Spotify is recommending you the new Cage the Elephant song because your friend John, whose musical taste is almost identical, has been listening to it a lot recently. Because the data is so much more complex, an interpretable decision tree for collaborative filtering may not be possible.

However, at a smaller scale, this is a relatively understandable technique. With a limited user base and song collection, like a classroom setting, an interpretable explanation of the mechanics of collaborative filtering is possible. They key contribution of this project to a students' understanding of collaborative filtering will be allowing them to clearly **visualize** why a recommendation system might select certain songs for them, and trace the **origins** of those recommendations.

Ideally, the level of detail in this explanation will be a choice given to the user, who will select whether they want to dive deep into matrix factorization or stay at the high-level visual tracing of collaborative filtering.

The basics of collaborative filtering are explained in [this](https://developers.google.com/machine-learning/recommendation/collaborative/basics) Google Machine Learning article.

### Content-Based Filtering

Content-based filtering can be used in conjunction with collaborative filtering. Content-based filtering is based on the actual audio characteristics of a track. For instance, a track's tempo is an audio characteristic. Companies like Spotify have attempted to create subjective metrics like happiness and energy and map them onto scalar values from 0 to 1.

Given sufficient data about a track's audio characteristics, content-based filtering looks at other tracks that seem to have similar characteristics.

The side effects of content-based filtering become more apparent when considering playlistification and the overall impact of streaming services on music.

### Playlistification

Playlistification refers to the dominant format in which music is consumed in the modern era: rather than an album or radio station, playlists have become the dominant method of listening to music. 35 million people follow the "Today's Top Hits" playlist on Spotify, many multiples of the regular listnership of the top music radio programs in the U.S.

<iframe data-testid="embed-iframe" style="border-radius:12px" src="https://open.spotify.com/embed/playlist/37i9dQZF1DXcBWIGoYBM5M?utm_source=generator&theme=0" width="100%" height="352" frameBorder="0" allowfullscreen="" allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture" loading="lazy"></iframe>

Most playlists Spotify offers, however, are marketed as giving you the perfect soundtrack for every "moment". This marketing strategy, positioning music as something that is suited for a particular occaison or mood, actually does meet a prominent user demand. Doing so at great scale in undoubtedly useful for most Spotify users.

The scale of this is illustrates by Spotify's relatively new "niche" mixes, which provide playlists of 50 tracks that are associated with an incredibly specific word or set of words, such as "Clowncore":

<iframe data-testid="embed-iframe" style="border-radius:12px" src="https://open.spotify.com/embed/playlist/37i9dQZF1EIdCJReXU4Hms?utm_source=generator&theme=0" width="100%" height="352" frameBorder="0" allowfullscreen="" allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture" loading="lazy"></iframe>

These playlists are personalized for every Spotify user, and they update daily. This means that Spotify has identified likely thousands of songs as "Clowncore", and it will suggest songs with that tag most closely related to your music taste (if you use Spotify, try clicking on the playlist to see what "Clowncore" recommendations are tailored for you).

### Modern Payola

The 

### Bias Toward Popular Music

### Conversion to Lean-Back
