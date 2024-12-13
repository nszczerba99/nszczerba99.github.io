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

## Research

The first step was to conduct user research to identify the most common pain points of the Spotify app. I **interviewed several individuals** and then synthesized the information into an **affinity diagram** to identify key patterns and insights.

<div style="padding:64.64% 0 0 0;position:relative;margin-bottom: 24px"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;border: 1px solid rgba(0, 0, 0, 0.1);" src="https://www.figma.com/embed?embed_host=share&url=https%3A%2F%2Fwww.figma.com%2Fboard%2FgyJSaVBMvXC0tN4Uggo998%2FSpotify-Redesign-Affinity-Diagram%3Fnode-id%3D0%253A1%26t%3DbTZ6O7bZ8Q91j7vo-1" allowfullscreen></iframe></div>

As illustrated above, users had numerous complaints across various areas of the app, with **podcasts** being a common source of frustration. Below are some **key highlights** of the most prevalent pain points.

{% include cards.html source=site.data.projects.spotify.problems %}

## Brainstorming

Once I pinpointed the most pressing issues to address, I delved into ideation to devise potential solutions. This phase involved **collaborative brainstorming session** with guidance from my mentor.

{% include animated_image.html src="https://i.imgur.com/oQUd7A8.jpg" alt="Brainstorming session" %}

Some solutions were readily apparent or had been previously suggested by users, while others required deeper consideration. By the end of our session, we managed to craft solutions for the most critical user issues (grey sticky notes in the [affinity map](#research)).


## Redesigning

During this phase, I utilized the *Figma* tool for high-fidelity prototyping. Below are a few of the changes I successfully designed.

### New logic inside a podcast

Previously, many podcasts were configured to display **only the latest episode at the top**, providing an easy shortcut to the most recent release. However, many users weren't up to date with their podcasts, so the latest episode wasn't relevant to them; they were more interested in **the last episode they had listened to**. On top of that, users often had to **scroll through a long list** of episodes (from newest to oldest) to find where they left off.

To address this, I added **a new tile** next to the *Latest episode* called *Continue listening*. This solution caters to both users interested in the latest episodes and those wanting to resume their last listened episode.

<div class="row mt-4">
    <div class="col-sm-12 col-md-6 wow animate__animated animate__fadeInLeft" data-wow-delay=".15s">
        <p class="lead text-center">Before</p>
        <img src="https://i.imgur.com/jPhPT2C.png" alt="Podcast page before">
    </div>
    <div class="col-sm-12 col-md-6 wow animate__animated animate__fadeInRight" data-wow-delay=".4s">
        <p class="lead text-center">After</p>
        <img src="https://i.imgur.com/OcJhlfd.png" alt="Podcast page's new layout">
    </div>
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
