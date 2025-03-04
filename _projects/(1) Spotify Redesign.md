---
name: Spotify Redesign
tools: []
image: https://i.imgur.com/KVVMtgb.png
description: Redesign of the Spotify Desktop App. New, improved version of the most popular music streaming platform.
---

{% include projects/project-navigation.liquid %}

![Spotify Redesign project thumbnail](https://i.imgur.com/81QiOBv.png)

{% include tags.liquid source=site.data.projects.spotify.tags %}

# Spotify Redesign

This project was part of a **mentorship program** at my workplace, where I was paired with an **experienced UX designer** to guide me through a design process. After some initial discussions, we decided to **redesign the Spotify Desktop App**. Over the next three months, I worked on this redesign, with my mentor providing advice and feedback throughout the journey.

## The challenge

<div class="row align-items-center">
    <div class="col-sm-3 col-12">
      {% include animated-image.liquid src="https://i.imgur.com/TSEpwpl.png" alt="A frustrated Spotify user struggling to navigate the app." %}
    </div>
    <div class="col-sm-9 col-12">
        Spotify is one of the most popular <strong>music streaming platforms</strong>, but it’s not without its <strong>pain points</strong>. Many users struggle with aspects of its interface, navigation, and discoverability. This project aimed to <strong>identify and address</strong> these <strong>common frustrations</strong>, enhancing the overall user experience to <strong>make Spotify more intuitive, enjoyable, and seamless</strong>.
    </div>
</div>

## My role

In this project, I took on the roles of both **UX Researcher** and **UX Designer**. I conducted **user research** to identify key pain points and **designed solutions** to enhance the overall experience of the app. My **mentor** provided **guidance** and oversight, acting as the **project lead**.

## Research and ideation

The first step was to conduct user research to identify the **most common pain points** of the Spotify app. I **interviewed several individuals** and then synthesized the information into an **affinity diagram** to identify key patterns and insights.

{% include projects/spotify/affinity-map-carousel.liquid %}

As illustrated above, users had numerous complaints across various areas of the app, with **podcasts** being a common source of frustration. Below are the most important **insights** from my research.

### Key insights

{% include cards.liquid source=site.data.projects.spotify.problems %}

<br/>

Once I pinpointed the most pressing issues to address, I delved into ideation to devise potential solutions. This phase involved **collaborative brainstorming session** with guidance from my mentor.

Some solutions were readily apparent or had been previously suggested by users, while others required deeper consideration. By the end of our session, we managed to craft solutions for the most critical user issues (grey sticky notes in the affinity map).

## Redesign

During this phase, I used *Figma* to create **mockups** and **high-fidelity prototypes**. Below are a few of the changes I successfully designed.

### New logic inside a podcast

Previously, many podcasts were configured to display **only the latest episode at the top**, providing an easy shortcut to the most recent release. However, many users weren't up to date with their podcasts, so the latest episode wasn't relevant to them; they were more interested in **the last episode they had listened to**. On top of that, users often had to **scroll through a long list** of episodes (from newest to oldest) to find where they left off.

To address this, I added **a new tile** next to the *Latest episode* called *Continue listening*. This solution caters to both users interested in the latest episodes and those wanting to resume their last listened episode.


<div class="wow animate__animated animate__fadeInLeft" data-wow-delay=".2s">
    <p class="lead text-center">Before</p>
    <img src="https://i.imgur.com/jPhPT2C.png" alt="Podcast page before">
</div>
<div class="wow animate__animated animate__fadeInRight mt-3 mb-5" data-wow-delay=".4s">
    <p class="lead text-center">After</p>
    <img src="https://i.imgur.com/OcJhlfd.png" alt="Podcast page's new layout">
</div>

To ensure the **responsiveness** of the app, here’s how this design **adapts** to **smaller screens**:

<div class="row row-cols-1 row-cols-md-2 mt-4 mb-3">
  <div class="col wow animate__animated animate__fadeInLeft" data-wow-delay=".2s">
    <p class="lead text-center">Before</p>
    <img src="https://i.imgur.com/VzOOVeK.png" alt="Podcast page on smaller screens before">
  </div>
  <div class="col wow animate__animated animate__fadeInRight" data-wow-delay=".4s">
      <p class="lead text-center">After</p>
      <img src="https://i.imgur.com/M7hyLub.png" alt="Podcast page's new layout on smaller screens">
  </div>
</div>

### Podcasts in folders

I also introduced a way for users to **group their podcasts**, not just individual episodes. Users could now add their desired podcasts to **folders**, similar to how they organize playlists.

 <div class="row mt-4">
    <div class="col-sm-12 col-md-6">
        {% include animated-image.liquid src="https://i.imgur.com/TSYI9Qr.png" alt="Folder with podcasts in a library" %}
    </div>
    <div class="col-sm-12 col-md-6">
        {% include animated-image.liquid src="https://i.imgur.com/A164nVp.png" alt="View inside a folder with podcasts" %}
    </div>
</div>

### Podcast new look

To address the common complaint about the lack of separation between music and podcasts, I ensured that podcast entities were easily **distinguishable** from playlists and other content.\
I proposed **three designs** for how podcasts/podcast episodes should be presented on the Home page.

{% include animated-image.liquid src="https://i.imgur.com/lX0UfBM.png" alt="Podcast new look" %}

### New Home sections

I added new Home sections featuring **podcast recommendations**, addressing another common user complaint about their absence.

In the designs presented below, you'll notice that I also added some **customization options** to Home sections:
- **drag icons** next to each section allowing users to reorder them
- **close buttons** letting users hide certain sections from the Home screen.

{% include animated-image.liquid src="https://i.imgur.com/JMXRQJN.png" alt="Suggested podcasts section" %}

{% include animated-image.liquid src="https://i.imgur.com/oSOIMdT.png" alt="More like X podcast section" %}


### *Choose what to see on Home* panel

Similarly, I designed a new "Choose what to see" panel, positioned at the bottom of the Home page. This feature would empower users to select which sections exactly they want to see on the Home page.

{% include animated-image.liquid src="https://i.imgur.com/WDhm5GR.png" alt="Choose what to see on Home panel" %}

### Excluding from recommendations

The **"Exclude from your taste profile"** option is currently available **only for playlists**. To address the issue of **poor recommendations**, I decided to expand this feature to include **artists and podcasts** as well.

#### Podcasts

{% include animated-image.liquid src="https://i.imgur.com/HdWfaq3.png" alt="'Exclude from your taste profile' option for podcasts" %}

#### Artists

{% include animated-image.liquid src="https://i.imgur.com/BRxck0S.png" alt="'Exclude from your taste profile' option for artists" %}

<br/>

### *Liked Songs* filters

I also introduced **filters to the *Liked Songs* playlist**, enabling users to organize songs by **artist or album**. This would provide a more efficient alternative to scrolling through a lengthy list of tracks.

I proposed **two solutions** for how this filtering could look like.

#### Version 1

<div style="padding:64.64% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/948506383?badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" frameborder="0" allow="autoplay; fullscreen; picture-in-picture; clipboard-write" style="position:absolute;top:0;left:0;width:100%;height:100%;" title="Spotify Liked Songs Redesign v1"></iframe></div><script src="https://player.vimeo.com/api/player.js"></script>

<br/>
<br/>

#### Version 2

<div style="padding:64.64% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/948504070?badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" frameborder="0" allow="autoplay; fullscreen; picture-in-picture; clipboard-write" style="position:absolute;top:0;left:0;width:100%;height:100%;" title="Spotify Liked Songs Redesign v2"></iframe></div><script src="https://player.vimeo.com/api/player.js"></script>

### Accessibility considerations

One of the **accessibility concerns** raised during the research was the absence of a **transcript option** for **podcasts**. Users with **speech impairments** or those less fluent in a language would greatly benefit from a **written version** of the podcast. Below are designs showing how this could be implemented, following the same format as the **song lyrics feature** for **consistency** across the app.

#### Podcast transcript feature

{% include animated-image.liquid src="https://i.imgur.com/HsCjkOI.png" alt="Podcast transcript option on the play bar" %}

{% include animated-image.liquid src="https://i.imgur.com/dKv6L7J.png" alt="Podcast transcript" %}

<br/>

## Testing

To evaluate my designs, I combined concept testing with A/B testing. I sent an online survey to users, requesting their feedback on my proposed solutions. The survey also included two polls: one for users to vote on their preferred *Liked Songs* prototype (version 1 or 2) and another to choose their favorite podcast design. The survey results are detailed below.

{% include projects/poll-results.liquid images=false title="Liked Songs filters" source=site.data.projects.spotify.liked-songs-res %}

{% include projects/poll-results.liquid images=true title="Podcast new look" source=site.data.projects.spotify.podcast-icons-res %}

As shown above, the winners turned out to be:
- Version 2 of *Liked Songs* filters
- Version 2 of the new podcast look.

Additionally, there were several comments on other design aspects. The "Choose what to see" panel on the Home screen received a lot of praise. However, it was suggested that the separation of podcasts and music still needed improvement, with recommendations to create separate Home and Search for these two categories.

## Takeaways

### Understanding user diversity

One of the key takeaways from this project was the realization of how **diverse** the **user base** can be, with different needs and preferences. For example, some users only used Spotify for **podcasts**, while others used it exclusively for **music**. This highlighted the importance of understanding various **user types** and their specific needs before jumping into the design process.

### Overcoming personal bias

Another valuable lesson was learning to combat my own **bias** as a Spotify user. While I have my own frustrations and pain points with the app, I had to remind myself that my **personal opinions** could not be the sole basis for the redesign. It was essential to focus on a wide range of **user experiences**, ensuring I didn’t prioritize my own needs above others’. This reinforced the importance of **user-centered design**, where insights from diverse users guide the solution.

### Motivation and enjoyment

On a positive note, being a **Spotify user** myself also provided **motivation** throughout the redesign process. My personal experience with the app made the project more **engaging**, and I found **joy** in tackling design challenges. This showed me that **UX design** can be both fun and rewarding when you’re deeply involved in solving real user problems.

### A valuable learning experience

Ultimately, this project was a fantastic **learning opportunity**. It taught me a lot about the **design process** and allowed me to explore **Figma’s features** in depth. I also received valuable **guidance** from my **mentor** throughout the project, which helped me deepen my understanding of UX design and refine my approach to **user-centered solutions**.

