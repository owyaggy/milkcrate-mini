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

> [!NOTE]
>
> <details>
>   <summary>A note about that data…</summary>
>   Spotify has followed a now well-established path in the industry: as a newcomer, they built out an excellent platform for interacting with and managing music, and made it publicly accessible via an API. As a result, creating a useful and interesting music tool in the past decade almost invariable involved the reliance on Spotify.
>   <br><br>
>     And, like quite a few before them, after they made it unviable to start a new platform because theirs was available for free, while they gained massive market share, they've begun to substantially restrict their API. The audio features described above were removed from the API in October 2024, and the ability to have more than 25 users sign-in to a Spotify-enabled app was essentially blocked in June 2025. In other words, it is functionally impossible to build an app based on Spotify any more.
> </details>

Given sufficient data about a track's audio characteristics, content-based filtering looks at other tracks that seem to have similar characteristics.

The side effects of content-based filtering become more apparent when considering playlistification and the overall impact of streaming services on music.

### Playlistification

Playlistification refers to the dominant format in which music is consumed in the modern era: rather than an album or radio station, playlists have become the dominant method of listening to music. 35 million people follow the "Today's Top Hits" playlist on Spotify, many multiples of the regular listnership of the top music radio programs in the U.S. (the most recent data in a cursory search was from 2017, which showed New York's WTLW had 5 million daily listeners).

<iframe data-testid="embed-iframe" style="border-radius:12px" src="https://open.spotify.com/embed/playlist/37i9dQZF1DXcBWIGoYBM5M?utm_source=generator&theme=0" width="100%" height="352" frameBorder="0" allowfullscreen="" allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture" loading="lazy"></iframe>

Most playlists Spotify offers, however, are marketed as giving you the perfect soundtrack for every "moment". This marketing strategy, positioning music as something that is suited for a particular occaison or mood, actually does meet a prominent user demand. Doing so at great scale in undoubtedly useful for most Spotify users.

The scale of this is illustrates by Spotify's relatively new "niche" mixes, which provide playlists of 50 tracks that are associated with an incredibly specific word or set of words, such as "Clowncore":

<iframe data-testid="embed-iframe" style="border-radius:12px" src="https://open.spotify.com/embed/playlist/37i9dQZF1EIdCJReXU4Hms?utm_source=generator&theme=0" width="100%" height="352" frameBorder="0" allowfullscreen="" allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture" loading="lazy"></iframe>

These playlists are personalized for every Spotify user, and they update daily. This means that Spotify has identified likely thousands of songs as "Clowncore", and it will suggest songs with that tag most closely related to your music taste (if you use Spotify, try clicking on the playlist to see what "Clowncore" recommendations are tailored for you).

According to *Mood Machine* by Liz Pelly, a book published earlier this year, these seemingly arbitrarily named "niches" are derived from analyzing user playlist data en masse, calculating word associations between playlist titles and songs on those playlists, and aggregating it into these (often bizarre) collections.

> [!NOTE]
>
> <details>
>   <summary>A note about Spotify's data collection on playlists</summary>
>   This is also a reflection on Spotify's use of user data: as they say in their developer [documentation](https://developer.spotify.com/documentation/web-api/concepts/playlists) "the notion of deleting a playlist is not relevant within the Spotify's [sic] playlist system". A playlist owner who removes their own playlist doesn't delete it, but merely unfollows it, while their data happily remains.
> </details>

The primary format for consuming music has evolved constantly over time, and the corresponding moves toward streaming and playlists may just be another entry in a long list of paradigm shifts. But this one feels different: never before has there been such tight vertical integration between the tastemakers and the purveyors of music. And never before have the tastemakers so effectively convinced listeners that they have complete control over what they listen to — that every song presented to them is the result of carefully-tuned algorithms with a listener's best interest at heart.

Spotify first made waves in algorithmic music recommendation with its introduction of "Discover Weekly" in 2015, a personalized playlist with new songs tailored to every single user. When listening to Discover Weekly, users may regard it as a good-faith (sometimes lacking, sometimes impressive) attempt at finding new songs for them. That is a form of trust, however small. But what if streaming companies decide to change their algorithms? Not only do users have fewer suitable alternatives — they simply may never know.

### Modern Payola

Payola is a term (and practice) that became infamous in the 20th century. Radio DJs would accept money in exchange for giving airtime to their benefactors (or their clients). This practice was eventually regulated out of prominent existence; the Federal Communications Commission has banned pay-for-play *without disclosure* since the 1960s.

Spotify has a program it markets to artists today called "Discovery Mode". It works by allowing artists to select certain eligible songs to participate in the program. Those songs will then get an algorithmic boost: on any algorithmic playlist (one that says "Made for You" in its tagline or song radio playlists, for example), they will be shown to users more often and higher up in the tracklist.

In exchange, Spotify takes a 30% cut from the (already measly) paychecks to artists. In a world where Spotify has commanding market share, forcing artists to succeed on Spotify for a chance at success, period, there is huge incentive for artists to participate.

### Bias Toward Popular Music

A new feature in music consumption introducted by streaming services is unavoidable knowledge of a track's popularity metrics. Spotify, and Apple Music to a lesser extent, highlight or provide stream counts for songs. These highlights may be intended to act as a sort of basic collaborative filtering – if many others think a song is good, it's likely you will too.

However, research has shown that the bias toward "popular" music is purely numbers-driven. A study collected listener data on a group of songs, allowing numbers to rise for the clear favorites. They then reversed those numbers and presented new listeners with the least popular songs masquerading as the most popular. The study found that listener behavior was identical with respect to popularity figures, meaning that listeners were essentially exclusively basing their decision on what to listen to based on popularity figures.

If the goal of listeners is simply to listen to what others listen to, this is perfectly valid. However, it seems likely that sometimes the signals given to an algorithm might not reflect what a user would consciously choose.

### Conversion to Lean-Back

The overarching concern in all of the above factors is that streaming services wield immense control over the world of music. They can strongly influence what  songs people listen to, and consequently how much different artists get paid. And the ability to change this paradigm is limited – streaming has made the dream of the "celestial jukebox", where any song is instantly at your fingertips, practically a reality. But for all of the benefits this provides, it has substantial costs too. People are dependent on these services, and their are few comparable alternatives.
