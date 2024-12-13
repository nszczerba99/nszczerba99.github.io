---
name: Spotify Redesign
tools: []
image: https://i.imgur.com/KVVMtgb.png
description: Redesign of the Spotify Desktop App. New, improved version of the most popular music streaming platform.
---

{% include projects/project_navigation.html %}

![Spotify Redesign project thumbnail](https://i.imgur.com/81QiOBv.png)

{% include tags.html source=site.data.projects.spotify.tags %}

# Spotify Redesign

## How it started

This project was part of a **mentorship program** at my workplace, where I was paired with an experienced UX designer to guide me through a design process. After some initial discussions, we decided to **redesign the Spotify Desktop App**. Over the next three months, I worked on this redesign, with my mentor providing advice and feedback throughout the journey.

## Research and Ideation

The first step was to conduct user research to identify the most common pain points of the Spotify app. I **interviewed several individuals** and then synthesized the information into an **affinity diagram** to identify key patterns and insights.

<div id="researchCarouselIndicators" class="carousel slide carousel-dark bg-light mt-1 mb-4">
  <div class="carousel-indicators">
    <button type="button" data-bs-target="#researchCarouselIndicators" data-bs-slide-to="0" class="active" aria-current="true" aria-label="Slide 1"></button>
    <button type="button" data-bs-target="#researchCarouselIndicators" data-bs-slide-to="1" aria-label="Slide 2"></button>
    <button type="button" data-bs-target="#researchCarouselIndicators" data-bs-slide-to="2" aria-label="Slide 3"></button>
    <button type="button" data-bs-target="#researchCarouselIndicators" data-bs-slide-to="3" aria-label="Slide 4"></button>
    <button type="button" data-bs-target="#researchCarouselIndicators" data-bs-slide-to="4" aria-label="Slide 5"></button>
  </div>
  <div class="carousel-inner">
    <div class="carousel-item active">
      <img src="https://i.imgur.com/78KFkEh.png" class="d-block mx-auto" height="700" alt="Users' issues with podcasts">
    </div>
    <div class="carousel-item">
      <img src="https://i.imgur.com/HnnW6a8.png" class="d-block mx-auto" height="700" alt="Users' issues with Home">
    </div>
    <div class="carousel-item">
      <img src="https://i.imgur.com/Ikr1wXe.png" class="d-block mx-auto" height="700" alt="Users' issues with Search">
    </div>
        <div class="carousel-item">
      <img src="https://i.imgur.com/Tuc1ZgR.png" class="d-block mx-auto" height="700" alt="Users' issues with Library">
    </div>
        <div class="carousel-item">
      <img src="https://i.imgur.com/EeoUA2B.png" class="d-block mx-auto" height="700" alt="Users' other issues">
    </div>
  </div>
  <button class="carousel-control-prev" type="button" data-bs-target="#researchCarouselIndicators" data-bs-slide="prev">
    <span class="carousel-control-prev-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Previous</span>
  </button>
  <button class="carousel-control-next" type="button" data-bs-target="#researchCarouselIndicators" data-bs-slide="next">
    <span class="carousel-control-next-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Next</span>
  </button>
</div>

As illustrated above, users had numerous complaints across various areas of the app, with **podcasts** being a common source of frustration. Below are some **key highlights** of the most prevalent pain points.

{% include cards.html source=site.data.projects.spotify.problems %}

Once I pinpointed the most pressing issues to address, I delved into ideation to devise potential solutions. This phase involved **collaborative brainstorming session** with guidance from my mentor.

Some solutions were readily apparent or had been previously suggested by users, while others required deeper consideration. By the end of our session, we managed to craft solutions for the most critical user issues (grey sticky notes in the affinity map).


## Redesigning

During this phase, I utilized the *Figma* tool for high-fidelity prototyping. Below are a few of the changes I successfully designed.

### New logic inside a podcast

Previously, many podcasts were configured to display **only the latest episode at the top**, providing an easy shortcut to the most recent release. However, many users weren't up to date with their podcasts, so the latest episode wasn't relevant to them; they were more interested in **the last episode they had listened to**. On top of that, users often had to **scroll through a long list** of episodes (from newest to oldest) to find where they left off.

To address this, I added **a new tile** next to the *Latest episode* called *Continue listening*. This solution caters to both users interested in the latest episodes and those wanting to resume their last listened episode.


<div class="wow animate__animated animate__fadeInLeft" data-wow-delay=".2s">
    <p class="lead text-center">Before</p>
    <img src="https://i.imgur.com/jPhPT2C.png" alt="Podcast page before">
</div>
<div class="wow animate__animated animate__fadeInRight mt-3" data-wow-delay=".5s">
    <p class="lead text-center">After</p>
    <img src="https://i.imgur.com/OcJhlfd.png" alt="Podcast page's new layout">
</div>


### Podcasts in folders

I also introduced a way for users to **group their podcasts**, not just individual episodes. Users could now add their desired podcasts to **folders**, similar to how they organize playlists.

 <div class="row mt-4">
    <div class="col-sm-12 col-md-6">
        {% include animated_image.html src="https://i.imgur.com/TSYI9Qr.png" alt="Folder with podcasts in a library" %}
    </div>
    <div class="col-sm-12 col-md-6">
        {% include animated_image.html src="https://i.imgur.com/A164nVp.png" alt="View inside a folder with podcasts" %}
    </div>
</div>

### Podcast new look

To address the common complaint about the lack of separation between music and podcasts, I ensured that podcast entities were easily **distinguishable** from playlists and other content.\
I proposed **three designs** for how podcasts/podcast episodes should be presented on the Home page.

<!-- ![Podcast new look](https://i.imgur.com/lX0UfBM.png) -->
{% include animated_image.html src="https://i.imgur.com/lX0UfBM.png" alt="Podcast new look" %}

### New Home sections

I added new Home sections featuring **podcast recommendations**, addressing another common user complaint about their absence.

In the designs presented below, you'll notice that I also added some **customization options** to Home sections:
- **drag icons** next to each section allowing users to reorder them
- **close buttons** letting users hide certain sections from the Home screen.

{% include animated_image.html src="https://i.imgur.com/JMXRQJN.png" alt="Suggested podcasts section" %}

{% include animated_image.html src="https://i.imgur.com/oSOIMdT.png" alt="More like X podcast section" %}


### *Choose what to see on Home* panel

Similarly, I designed a new "Choose what to see" panel, positioned at the bottom of the Home page. This feature would empower users to select which sections exactly they want to see on the Home page.

{% include animated_image.html src="https://i.imgur.com/WDhm5GR.png" alt="Choose what to see on Home panel" %}


### *Liked Songs* filters

I also introduced **filters to the *Liked Songs* playlist**, enabling users to organize songs by **artist or album**. This would provide a more efficient alternative to scrolling through a lengthy list of tracks.

I proposed **two solutions** for how this filtering could look like.

#### Version 1

<div style="padding:64.64% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/948506383?badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" frameborder="0" allow="autoplay; fullscreen; picture-in-picture; clipboard-write" style="position:absolute;top:0;left:0;width:100%;height:100%;" title="Spotify Liked Songs Redesign v1"></iframe></div><script src="https://player.vimeo.com/api/player.js"></script>

<br/>
<br/>

#### Version 2

<div style="padding:64.64% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/948504070?badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" frameborder="0" allow="autoplay; fullscreen; picture-in-picture; clipboard-write" style="position:absolute;top:0;left:0;width:100%;height:100%;" title="Spotify Liked Songs Redesign v2"></iframe></div><script src="https://player.vimeo.com/api/player.js"></script>

## Testing

To evaluate my designs, I combined concept testing with A/B testing. I sent an online survey to users, requesting their feedback on my proposed solutions. The survey also included two polls: one for users to vote on their preferred *Liked Songs* prototype (version 1 or 2) and another to choose their favorite podcast design. The survey results are detailed below.

{% include poll_results.html images=false title="Liked Songs filters" source=site.data.projects.spotify.liked-songs-res %}

{% include poll_results.html images=true title="Podcast new look" source=site.data.projects.spotify.podcast-icons-res %}

As shown above, the winners turned out to be:
- Version 2 of *Liked Songs* filters
- Version 2 of the new podcast look.

Additionally, there were several comments on other design aspects. The "Choose what to see" panel on the Home screen received a lot of praise. However, it was suggested that the separation of podcasts and music still needed improvement, with recommendations to create separate Home and Search for these two categories.
