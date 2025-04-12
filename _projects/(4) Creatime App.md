---
name: Creatime App
tools: []
image: https://i.imgur.com/GiOkn68.png
description: A mobile app that helps tutor adults in creativity.
---

{% include projects/project-navigation.liquid %}

![Creatime app project thumbnail](https://i.imgur.com/GiOkn68.png)

{% include tags.liquid source=site.data.projects.creatime.tags %}

# Creatime App

This project was the capstone of my ***Google UX Design Professional Certificate*** coursework, where I **applied** and synthesized **everything I learned** throughout the program.

## The challenge

From the challenges available in the course, I chose:

<blockquote class="blockquote">
    <p><em>Design a way to help tutor adults in creativity.</em></p>
</blockquote>

This topic stood out to me because I found it **personally compelling**, and I knew my **friends would make great target users** for research.  

<div class="row align-items-center">
    <div class="col-md-2 col-sm-4 col-12">
      {% include animated-image.liquid src="https://i.imgur.com/SzCVegF.png" alt="A frustrated adult struggling to find time and motivation for creative pursuits." %}
    </div>
    <div class="col-md-10 col-sm-8 col-12">
        Being <strong>creative as an adult</strong> is challenging. <strong>Full-time jobs</strong> leave <strong>little time and energy</strong> for creative pursuits, and many people struggle with <strong>motivation and self-doubt</strong>. My goal was to address these obstacles by designing a solution that helps adults <strong>reclaim their creativity</strong> in today’s <strong>fast-paced world</strong>.
    </div>
</div>

## My role

{% include projects/creatime/my-roles.liquid %}

Since this project was a part of my coursework, I took ownership of the entire **design process** from start to finish. This included conducting **user research**, structuring the app’s **information architecture**, designing its **interactions** and **layout**, and progressing through **wireframing**, **prototyping**, and **UI refinement**. I applied key **visual design principles** such as **color**, **typography**, and **component design** to create a polished final product.

## User research

I sent a **survey** to **9 participants** to identify the **challenges** hindering their creative development, understand the **support and resources they need** to overcome these obstacles, and  gather insights into their **preferred tools or features**. Below are the charts displaying some of their responses.

{% include projects/poll-results.liquid title="What are your reasons for wanting to develop your creativity?" source=site.data.projects.creatime.poll-results.reasons %}

{% include projects/poll-results.liquid title="What challenges or obstacles make it difficult for you to develop your creativity?" source=site.data.projects.creatime.poll-results.challenges %}

{% include projects/poll-results.liquid title="What support or resources would help you better develop your creativity?" source=site.data.projects.creatime.poll-results.resources %}

I compiled all the survey data into an **affinity map**, identifying **patterns and common themes**.

{% include animated-image.liquid src="https://i.imgur.com/6ZcljNd.png" alt="Affinity map" %}

### Key insights

{% include projects/insights.liquid source=site.data.projects.creatime.insights1 %}

### Target users

Based on my research, I identified **two** unique user personas: **Ji-hye and Rohan**.

{% include animated-image.liquid src="https://i.imgur.com/J2G9iPN.png" alt="User persona: Ji-hye Kim" %}

{% include animated-image.liquid src="https://i.imgur.com/bFoZV0Y.png" alt="User persona: Rohan Patel" %}

<br/>
Based on the user personas, I outlined the following **problem statements**:

{% include projects/problem-statements.liquid source=site.data.projects.creatime.problem-statements%}

## Competitors

The next step involved a **competitive audit**, where I analyzed my app's competitors to uncover **patterns** and **potential market gaps**. I've outlined **four competitors** and the **key insights** from this review below.

{% include projects/creatime/competitors.liquid source=site.data.projects.creatime.competitors%}

### Common themes & market gaps

<strong class="text-themed-purple">Diverse learning formats:</strong> While most competitors primarily rely on video-based learning, there’s an opportunity to innovate with more interactive, immersive, and hands-on experiences that bridge the gap between theory and real-world application.

<strong class="text-themed-purple">Affordability & accessibility:</strong> MasterClass’ premium pricing may be a barrier for some learners, while Skillshare's expansive library can feel overwhelming for those seeking focused, expert-led content.

<strong class="text-themed-purple">Motivation gap:</strong> Platforms often overlook the importance of motivation. Incorporating features like quotes, badges, and progress recognition can keep learners engaged and motivated, helping them celebrate milestones and stay committed to their creative journeys.

<strong class="text-themed-purple">Lack of focus on fun & relaxation:</strong> While most platforms emphasize learning new skills, there’s a gap in offering spaces for creative expression and relaxation. A platform that encourages playfulness, exploration, and stress-free creativity could appeal to users seeking a more enjoyable, low-pressure learning experience.

---

<div class="alert alert-primary">
    There’s a need for a platform that offers affordable content across a <strong>well-defined range</strong> of creative topics, <strong>without overwhelming</strong> users, while emphasizing <strong>fun and relaxation</strong>. A <strong>strong community</strong> and <strong>motivational features</strong> would further enhance the experience.
</div>

## Crazy Eights

Next, keeping the **user's needs** in mind, I performed the **"Crazy Eights"** exercise to generate a **wide range of ideas**, then **reviewed** them to select the most promising ones.

{% include animated-image.liquid src="https://i.imgur.com/SSoYbaF.jpeg" alt="Crazy Eights exercise" %}

## Understanding user flows

I mapped out the **key user flows**, such as completing a lesson, or posting a user's work. Below is one of the user flows I outlined, illustrating the process of **finding and enrolling in a course**.

{% include animated-image.liquid src="https://i.imgur.com/vjrxYjo.png" alt="User flow of finding a course and enrolling in it." %}

## Wireframing

First, I created **paper wireframes** for the **key user flows** I had previously outlined.

{% include projects/creatime/paper-wireframes.liquid %}

Then, based on the paper wireframes, I created **digital versions** that were slightly more detailed and refined.

{% include projects/creatime/digital-wireframes.liquid %}

## Usability study

{% include projects/usability-study-info.liquid source=site.data.projects.creatime.usability-study-info %}

For the study, I used a **low-fidelity prototype**, created from my digital wireframes, to simulate **key user flows**. Participants **performed tasks** such as finding and enrolling in a course, completing a lesson and earning a badge, or posting a picture to the community.

### Insights

{% include projects/insights.liquid source=site.data.projects.creatime.insights2 %}

I **outlined solutions** for **each user pain point** and then moved on to developing the **visual design** and **app mockups** that bring those solutions to life.

## Designing UI

In designing the **UI**, I aimed to create an experience that feels **creative, playful, and fun** - more like a **game** than a pressured learning tool. I chose a **bright color palette** to reinforce this feeling and intentionally incorporated **game-like elements** throughout. For example, **ratings** use **puzzle pieces** instead of stars, **lessons** resemble a **board game**, and **challenges** are styled like **game cards**. Even the **logo** features **dot elements** that subtly reference **board game mechanics**, mirroring the **course structure**. My goal was to keep everything **visually engaging, lively, and stress-free**.  

{% include animated-image.liquid src="https://i.imgur.com/mGRTRqw.png" alt="Stickersheet: Part 1" %}

{% include animated-image.liquid src="https://i.imgur.com/wJw2uJN.png" alt="Stickersheet: Part 2" %}

## Final designs

{% include projects/creatime/mockups1.liquid %}

{% include projects/creatime/mockups2.liquid %}

The final designs effectively **address** the key **user pain points** identified in the **usability study**.

To resolve complaints about the **lack of an option to dismiss the "Challenges Unlocked" popup**, a **close button** was added, giving users more control over their experience.

To clarify where **pinned posts** go, a **confirmation message** now appears after pinning, informing users about the **Inspiration Board** and providing a link to it.

Lastly, the inconsistent **"Mark as Done"** button placement in **lessons** and **challenges** was standardized. Both now feature a **floating button** at the **bottom of the screen**, ensuring consistency. This placement encourages users to read the lesson content before marking it as done, while also giving returning challenge users easy access to the button, without the need to scroll.

### App prototype

Based on the mockups, I created a **high-fidelity prototype** showcasing the key **user flows**, presented in the video below.

<div class="container ratio ratio-16x9">
    <iframe width="1247" height="703" src="https://www.youtube.com/embed/PUwxPgA2kQw" title="Creatime Mobile App Prototype" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
</div>

### Meeting user needs

{% include projects/insights.liquid source=site.data.projects.creatime.insights3 %}

## Lessons learnt

### The value of paper wireframes  
During the early stages of this project, I dedicated significant time to creating **paper wireframes** for each screen, exploring **multiple variations** before selecting the best design. Although this process was time-consuming, it proved invaluable. By making **key design decisions** early on, I established a **strong foundation** for the subsequent stages of the project, which ultimately **saved time later**. In future projects, I’ll stay committed to using **paper wireframes** to ensure a solid start to the design process.

### Balancing quantitative and qualitative data  
In this project, I relied heavily on a **survey** for foundational **research**, which provided useful **quantitative data** - mainly from users selecting **pre-written options**. However, this approach limited my understanding of users’ deeper issues, as it didn't capture their thoughts and experiences in **their own words**. Moving forward, I plan to incorporate more **qualitative data**, such as **user interviews**, to gain a fuller understanding of their needs and pain points. This will allow for more **empathetic**, user-driven design decisions.

### AI-generated text over *Lorem Ipsum*  
For this project, I decided to replace the traditional ***Lorem Ipsum*** placeholder text with **AI-generated content**. This decision was inspired by a **course** I took on AI, which gave me new insights into its potential. Using AI-generated text not only **saved time** but also ensured that the content felt more **relevant and realistic**. Additionally, *Lorem Ipsum* can sometimes **confuse users** who aren't familiar with it, and using meaningful text helped create a **more authentic experience**. Going forward, I’ll continue utilizing AI-generated content in my future projects.