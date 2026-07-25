---
name: Qualtrics Color Tokens
tools: []
image: https://cdn.jsdelivr.net/gh/nszczerba99/ux-portfolio-images@main/projects/color-tokens/cover.webp
description: Collaborated with UX design to implement a scalable color token system in code.
---

{% include projects/project-navigation.liquid %}

![Color Tokens project thumbnail](https://cdn.jsdelivr.net/gh/nszczerba99/ux-portfolio-images@main/projects/color-tokens/cover.webp)

{% include tags.liquid source=site.data.projects.color-tokens.tags %}

# Qualtrics Color Tokens

This project was completed during my time as a **Software Engineer** at **Qualtrics**, where I led the engineering implementation of a **new color token system**. Working closely with a **UX designer**, we created a shared foundation that aligned design and development around a single source of truth.

## The challenge

<div class="row">
    <div class="col-md-6 col-12">
      {% include animated-image.liquid src="https://cdn.jsdelivr.net/gh/nszczerba99/ux-portfolio-images@main/projects/color-tokens/challenge.webp" alt="Colors scattered randomly on a canvas." %}
    </div>
    <div class="col-md-6 col-12">
      <p class="lead">Colors scattered across multiple codebases</p>
      <p>
        The existing color system lacked consistency. Multiple teams maintained their own token libraries, alongside additional hardcoded values, leading to fragmentation and no single source of truth.
      </p>
      <br/>
      <p class="lead">Disconnect between design and development</p>
      <p>
          Color names differed across Figma and the codebase, which led to misunderstandings between designers and engineers.
      </p>
      <br/>
      <p class="lead">Limited color scalability</p>
      <p>
          There was no easy way to update the color of a specific UI element across multiple parts of the system or support dark mode.
      </p>
      <br/>
    </div>
</div>

<p>The goal was to create a <strong class="text-themed-green">unified, central color token system</strong> as a single source of truth across the <strong>codebase and design</strong>, ensuring <strong>consistency</strong> and <strong>scalability</strong> across the product.
</p>

## My role

<div class="row align-items-center">
    <div class="col-md-1 col-sm-4 col-12">
      {% include animated-image.liquid src="https://cdn.jsdelivr.net/gh/nszczerba99/ux-portfolio-images@main/projects/color-tokens/code.webp" alt="Programming symbol" %}
    </div>
    <div class="col-md-11 col-sm-6 col-12">
        I led the <strong>software engineering</strong> side of the project in close <strong>collaboration with a UX designer</strong>. My responsibilities included defining the token architecture, implementing the color tokens in code and aligning the engineering system with the design tokens in Figma.
    </div>
</div>

## Approach

The new color system was built around two types of tokens: base tokens and aliases.

<p class="lead">1) Base tokens</p>

Base tokens represent the raw color palette (e.g. `blue-100` to `blue-1000`) and contain only color values.

{% include animated-image.liquid src="https://cdn.jsdelivr.net/gh/nszczerba99/ux-portfolio-images@main/projects/color-tokens/base-tokens.webp" alt="" %}

<p class="lead">2) Aliases</p>

Aliases are semantic tokens (e.g. `text-brand-default`, `border-danger-hover`) that describe how a color is used throughout the interface. Each alias references a base token. These are the tokens developers should use throughout the codebase.

{% include animated-image.liquid src="https://cdn.jsdelivr.net/gh/nszczerba99/ux-portfolio-images@main/projects/color-tokens/aliases.webp" alt="" %}

### Advantages

<div class="row">
    <div class="col-md-7 col-sm-6 col-12">
      <h4>Flexible color updates</h4>
      <p>
        This separation creates a layer of abstraction between the color palette and implementation. Instead of updating a color everywhere it's applied, we can simply change the base token assigned to an alias, automatically updating every element that uses that semantic role — for example, all button hover states. This makes color changes targeted, predictable, and much easier to maintain as the product grows.
        </p>
    </div>
    <div class="col-md-5 col-sm-6 col-12">
      {% include animated-image.liquid src="https://cdn.jsdelivr.net/gh/nszczerba99/ux-portfolio-images@main/projects/color-tokens/flexible.webp" alt=""%}
    </div>
</div>

<div class="row">
    <div class="col-md-3 col-sm-6 col-12 order-sm-1 order-2">
      {% include animated-image.liquid src="https://cdn.jsdelivr.net/gh/nszczerba99/ux-portfolio-images@main/projects/color-tokens/dark-light-modes.webp" alt="" %}
    </div>
    <div class="col-md-9 col-sm-6 col-12 order-sm-2 order-1">
      <h4>Dark mode support</h4>
      <p>
        This same architecture also makes future dark mode support possible. In dark mode, base tokens automatically switch to their <strong>symmetrical</strong> counterparts — for example, <code class="highlighter-rouge">blue-100</code> switches to <code class="highlighter-rouge">blue-1000</code>, and <code class="highlighter-rouge">blue-200</code> switches to <code class="highlighter-rouge">blue-900</code>. This keeps the system consistent, simple, and well-organized.
      </p>
    </div>
</div>

## The process

{% include cards-2-cols.liquid source=site.data.projects.color-tokens.process %}

## Results

The project established a **centralized color token system** that serves as a single **source of truth** across design and development. By replacing fragmented color definitions with semantic tokens, the system became **more consistent, scalable, and easier to maintain**.

The new token system became part of the **public Qualtrics Design System** and is available for developers worldwide through the official npm package.

- **npm package**: <https://www.npmjs.com/package/@qualtrics/ui-react/>

- **Official documentation**: <https://designsystem.qualtrics.com/design-tokens/color-tokens/>

{% include animated-image.liquid src="https://cdn.jsdelivr.net/gh/nszczerba99/ux-portfolio-images@main/projects/color-tokens/documentation.webp" alt="Color tokens section of the Qualtrics Design System documentation" %}


## Takeaways

### UX–engineering collaboration

One of the biggest lessons was the importance of close collaboration between UX and engineering. Regular feedback loops throughout the project helped ensure the final implementation remained consistent, practical, and aligned with the original design intent.

### Designing for scalability

I gained practical experience designing and implementing a scalable color token architecture based on base and semantic tokens, and learned how this approach supports long-term maintainability.

### Building for future theming

This project deepened my understanding of how a well-structured token system enables features like dark mode without increasing implementation complexity.
