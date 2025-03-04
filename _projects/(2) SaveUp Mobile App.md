---
name: SaveUp Mobile App
tools: []
image: /assets/img/group_savings_cover.png
description: Mobile app that helps friend or family groups save up for a common goal.
---

{% include projects/project-navigation.liquid %}

![SaveUp app project thumbnail](https://i.imgur.com/XcBBke0.png)

{% include tags.liquid source=site.data.projects.saveup-mobile.tags %}

# SaveUp Mobile App

I designed the *SaveUp* mobile app as part of my **coursework** for the ***Google UX Design Professional Certificate***. This project was a **hands-on learning experience** that allowed me to apply new UX concepts and skills in real time as I advanced through the course.

## The challenge

As part of the course, I was given a list of design challenges to choose from. I selected the following:

<blockquote class="blockquote">
    <p><em>Design an app and a responsive website that help friend or family groups manage a household budget and save up for a common goal (such as a vacation).</em></p>
</blockquote>

Saving money can be challenging on its own, but saving as a group adds even more complexity. Conversations about money can be uncomfortable, and coordinating multiple people requires organization and transparency. My goal was to design an app that simplifies group savings, making it easier for friends and family to set goals, track contributions, and stay motivated together.

## My role

{% include projects/saveup-mobile/my-roles.liquid%}

Since this project was part of **my coursework**, I handled **the entire design process** from **start to finish**. This included conducting user research, designing the app’s structure and interactions, and refining the UI with thoughtful choices in color, typography, and overall visual design.

## Foundational Research

The course provided a set of fictional user profiles, which served as the foundation for my research. Using empathy exercises, I analyzed these profiles to better understand user needs, motivations, and pain points. This process led to the creation of the following empathy maps and user personas.

{% include projects/saveup-mobile/empathy-maps.liquid %}

### Target users

I identified **two** distinct target users: Alex and Sofia.

<div class="row row-cols-1 row-cols-md-2 mb-4">
    <div class="col">
        {% include animated-image.liquid src="https://i.imgur.com/lkslwDX.png" alt="User persona: Alex" %}
    </div>
    <div class="col">
        {% include animated-image.liquid src="https://i.imgur.com/a24hsSe.png" alt="User persona: Sofia" %}
    </div>
</div>

I compiled Alex and Sofia's key problems and needs into **user stories**, which are presented below.

{% include cards.liquid source=site.data.projects.saveup-mobile.user-stories %}

## Coming up with ideas

### User journeys

For both user personas, I mapped out their **user journeys** to understand **their emotions** at each stage and identify **key features the app needed** to effectively **address their challenges**.

{% include projects/journey-map.liquid source=site.data.projects.saveup-mobile.journey-maps.alex%}
{% include projects/journey-map.liquid source=site.data.projects.saveup-mobile.journey-maps.sofia%}

### Rapid sketching

I sketched my various **ideas** using the **"Crazy Eights"** exercise. Afterward, I analyzed which concepts had the **most potential** and determined the best direction for the app.

{% include animated-image.liquid src="https://i.imgur.com/rlSBW8C.jpeg" alt="Rapid sketching exercise" %}

## Wireframing

Using *Figma* tool, I created **early app designs** along with a **low-fidelity prototype** showcasing the app's functionality.

### Goal and personal spaces

To structure savings effectively, I introduced **goal spaces** - shared spaces where a **group** saves together for a common goal - and a **personal space**, a **private** area where users can track their income and **personal transactions**, such as salaries or grocery expenses.

In contrast, **group transactions** involve expenses **shared** between members saving for a common goal. For example, if one person covers a cost for others, the app helps manage **balances** to settle debts.

To enhance the experience, I incorporated detailed **financial analysis** within both goal and personal spaces. In the goal space, this includes features like predicting when a goal will be reached and automating the saving process to help users stay on track.

{% include projects/saveup-mobile/wireframes1.liquid %}

### Subgoals

To make large goals more manageable, I added the ability to create **subgoals**, allowing users to break down a main goal into **smaller milestones**. For instance, a vacation goal could include subgoals like booking a hotel or purchasing plane tickets.

### Customization

I designed several **customization options** to accommodate different saving preferences:
- **Goal Prioritization**: Users can choose between **saving for all goals and subgoals simultaneously** or following a **queue-based approach** - where savings are allocated to the first goal, then the second, and so on
  
- **Contribution Style**: Contributions can be **equal**, meaning everyone contributes the same amount, or **flexible**, where members contribute whatever they can until the goal is met.
  
- **Visibility Mode**: Users can opt for **public** mode, where everyone's individual savings are visible, or **private** mode, where only the total group savings amount is displayed.

These features ensure that the app can adapt to **different group dynamics** and financial habits, making collaborative saving more transparent and efficient.

{% include projects/saveup-mobile/wireframes2.liquid %}


## First usability study

Using the **low-fidelity prototype**, I conducted a **usability study** with **five participants**. The details of the study are outlined below.

{% include projects/saveup-mobile/usability-study-1.liquid %}

Later, I organized all my findings into an **affinity diagram** and identified **common themes**.

{% include animated-image.liquid src="https://i.imgur.com/fYqcApW.png" alt="Affinity diagram" %}

### Key insights

I uncovered several key insights through my research, which are outlined below.

{% include projects/insights.liquid source=site.data.projects.saveup-mobile.insights %}

I **updated the designs** to address the identified pain points and then started working on **mockups** that more closely aligned with the final product.

## Visual design

Before creating the mockups, I focused on the **visual design** of the app, selecting the color palette, typography, and iconography. I also defined key navigation elements and UI components that would be used consistently throughout the app, ensuring a cohesive and user-friendly experience.

{% include animated-image.liquid src="https://i.imgur.com/XxdVMjk.png" alt="Stickersheet: Part 1" %}
{% include animated-image.liquid src="https://i.imgur.com/Rj3JItD.png" alt="Stickersheet: Part 2" %}

After finalizing the visual design elements, I was able to create the app’s mockups.

## Second usability study

From the mockups, I developed a **high-fidelity prototype**, which I then used for the **second usability study**.

{% include projects/saveup-mobile/usability-study-2.liquid %}

### Results

#### Misunderstood goal modes

The study revealed that users are still **confused** about **goal modes** (*Goal Contribution Style* and *Savings Visibility Mode*) and their purpose.To improve clarity, I rewrote the mode **descriptions** in more **user-friendly** language and added visual **illustrations** for better understanding.

<div class="row my-5">
    <div class="col-md-6 wow animate__animated animate__fadeInLeft" data-wow-delay=".2s">
        <p class="lead text-center">Before</p>
        <img src="https://i.imgur.com/0YgECy8.png" alt="Goal modes before" class="phone-rounded">
    </div>
    <div class="col-md-6 wow animate__animated animate__fadeInRight" data-wow-delay=".4s">
        <p class="lead text-center">After</p>
        <img src="https://i.imgur.com/K47oNoB.png" alt="Goal modes' new look" class="phone-rounded">
    </div>
</div>

#### Unnecessary "Adjust required contribution" settle option

Another insight was that most users **don’t use or understand** the **"Adjust required contributions"** option to **settle balances**.

Instead of generating transfers to settle balances, this option adjusted each member's required contributions toward the goal. This meant that a member with more debt would need to contribute a higher amount, while the member who was owed would have a reduced savings requirement.

I’ve decided to **remove** this option from the app since it caused a lot of **confusion** without providing much value.

<div class="row my-5">
    <div class="col-md-6 wow animate__animated animate__fadeInLeft" data-wow-delay=".2s">
        <p class="lead text-center">Before</p>
        <img src="https://i.imgur.com/I5n0lqE.png" alt="Balance section before">
    </div>
    <div class="col-md-6 wow animate__animated animate__fadeInRight" data-wow-delay=".4s">
        <p class="lead text-center">After</p>
        <img src="https://i.imgur.com/9Rm9ACc.png" alt="Balance section's new look">
    </div>
</div>

#### Overall feedback

{% include projects/poll-results.liquid images=false title="I thought the app was easy to use." source=site.data.projects.saveup-mobile.sus.res-1%}
{% include projects/poll-results.liquid images=false title="I think that I would use this app frequently." source=site.data.projects.saveup-mobile.sus.res-2%}

The SUS (System Usability Scale) questionnaire feedback was **generally positive**, with most users agreeing that the app is **easy to use**. However, they indicated that they **wouldn’t** necessarily **use it frequently**, which is an area worth exploring for **future improvements**.

## Final designs

In my final designs, I **addressed** all the **insights** gathered from **previous user studies**. Key improvements include **clearer visual distinctions** between the **goal and personal spaces**.

I also simplified the interface by replacing the **identical plus buttons** for adding goals and transactions. Now, each button includes **descriptive text labels** to clearly indicate their specific functions.

To further enhance clarity, I **replaced** the **"Goal Prioritization" button** with a **dropdown menu**, clearly **labeled** to explain its function.

Lastly, based on user feedback, I moved the ***Balance*** section from the ***Overview*** tab to the ***Group Transactions*** tab, as users found its original location unintuitive.

{% include projects/saveup-mobile/mockups1.liquid %}

### Permission System

Based on previous **feedback** highlighting that the app's **permissions were too lenient**, I introduced a **privilege system** with two user roles: **admins** and **participants**.  

- **Admins** have full control over the goal. They can edit the goal, add subgoals, settle all balances, and delete the goal.  
- **Participants** have more limited permissions. They cannot edit the goal, add subgoals, or delete it. However, they can add group transactions, settle balances involving themselves, and leave the goal if needed.  

This system ensures better structure and control over group savings while maintaining flexibility for participants.

{% include projects/saveup-mobile/mockups2.liquid %}

<div class="row row-cols-1 row-cols-md-2 row-cols-lg-3 justify-content-center mb-5">
    <div class="col">
        <h3 class="text-center mt-5 mb-4">App Prototype</h3>
        <div style="padding:205.64% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/1062412072?badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" frameborder="0" allow="autoplay; fullscreen; picture-in-picture; clipboard-write; encrypted-media" style="position:absolute;top:0;left:0;width:100%;height:100%;" title="SaveUp Mobile App Prototype"></iframe></div><script src="https://player.vimeo.com/api/player.js"></script>
    </div>
</div>

## Takeaways  

### Designing for Group Savings  
This project deepened my understanding of the unique challenges in group saving - such as the need for **transparency, automation, and seamless collaboration**. I also learned that even when an app includes analytical and math-heavy features, it must remain **intuitive and jargon-free** to ensure usability for all.  

### Visual & Interaction Design  
While crafting the UI, I strengthened my understanding of **visual design principles**, including typography, spacing, and color palette creation. This experience reinforced how **thoughtful design choices impact clarity, engagement, and overall user experience**.  

### Enhancing My UX Research Process  
This project sharpened my **research planning and note-taking** skills, allowing me to **better structure insights and translate them into actionable design decisions**. I also refined my approach to **organizing and prioritizing user feedback**, making the research process more efficient.  

### Reducing Bias for Better Insights  
To improve research accuracy, I explored different strategies to **mitigate bias**, such as using **open-ended questions and neutral framing** to encourage **genuine, unbiased responses**. This helped me uncover **more authentic user needs**, ultimately leading to a more user-centered design.  

