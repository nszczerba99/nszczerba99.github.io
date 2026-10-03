---
name: ERP Side Panels Redesign
tools: []
image: https://cdn.jsdelivr.net/gh/nszczerba99/ux-portfolio-images@main/projects/erp-panels/cover.webp
description: "Redesign of the side panels in Comarch ERP Enterprise: their behavior, a new table data organization panel, and the linked documents panel."
---

{% include projects/project-navigation.liquid %}

![ERP side panels redesign project thumbnail](https://cdn.jsdelivr.net/gh/nszczerba99/ux-portfolio-images@main/projects/erp-panels/cover.webp)

{% include tags.liquid source=site.data.projects.erp-panels.tags %}

# ERP Side Panels Redesign

At **Comarch**, I was assigned to the redesign of **Comarch ERP Enterprise (CEE)** — a large, mature **ERP system** used daily by professionals who process **thousands of documents**: sales orders, deliveries, invoices. We were a **team of two designers** — a senior UX designer and me — and the effort began with the **Sales Order demo**: a redesign of the Sales orders feature, built on the **Comarch Design System**.

Most of that groundwork was in place before I joined. Once on board, I worked on the redesign alongside my teammate. This case study covers my work on the **side panel system**, internally known as **dockable views**.

## The context

Why a redesign? CEE has grown with its market for **many years**, and the current interface shows its age: **outdated visuals**, **unintuitive interactions**, and functionality hidden behind **cryptic icons**. Earlier **user research** confirmed the cost — users spend **a lot of time just learning the application**.

One look at the current interface shows why. It is **extremely information-dense**, with **no clear page hierarchy** — every control carries the same visual weight, so nothing guides the eye. The layout isn't something a user can figure out; it has to be **learned**:

{% include animated-image.liquid src="https://cdn.jsdelivr.net/gh/nszczerba99/ux-portfolio-images@main/projects/erp-panels/legacy-sales-orders.webp" alt="The current CEE interface: a dense Sales orders list with a large filter section and no clear hierarchy." %}

A broader **redesign initiative** was already underway: a new, modern layout for the Sales orders area had been proposed, refreshing the **visual language** and **navigation**:

{% include animated-image.liquid src="https://cdn.jsdelivr.net/gh/nszczerba99/ux-portfolio-images@main/projects/erp-panels/demo-sales-orders.webp" alt="The redesigned Sales orders list from the demo — the starting point before my work." %}

The demo was still being improved upon, with a lot of areas left to polish — one of them being the **side panels**. In CEE, panels are how users reach **contextual tools** without leaving their work — search, messages, tasks, favorites, and more. They are opened from **icon toolbars** docked to the edges of the screen — right, left, or bottom — and can be **pinned** and **resized**.

<div class="row align-items-center">
    <div class="col-md-3 col-sm-4 col-12">
      {% include animated-image.liquid src="https://cdn.jsdelivr.net/gh/nszczerba99/ux-portfolio-images@main/projects/erp-panels/legacy-panel-before.webp" alt="A dockable view panel in the current CEE interface, with small cryptic icons in its header." %}
    </div>
    <div class="col-md-9 col-sm-8 col-12">
        The existing panel system was <strong>powerful</strong>, but — like the rest of the application — its interface was <strong>outdated</strong> and <strong>not user-friendly</strong>: icons and controls were <strong>cryptic</strong>, and configuration was <strong>hard to discover</strong> and, once found, <strong>hard to figure out</strong>. The side panels were due for the same rethink the rest of the demo was getting.
    </div>
</div>

## The challenge

The task was bigger than a facelift. It fell into **three parts**:

{% include cards-3-cols.liquid source=site.data.projects.erp-panels.challenge %}

## My role

{% include projects/erp-panels/my-roles.liquid %}

I was responsible for the **UX and UI design** of the panel system within the Sales orders redesign. This included **auditing** the current dockable views, defining the **interaction model** (opening, closing, pinning, resizing, splitting), and designing the **panel components**. I also designed two specific dockable views: the **table data organization** panel and the **linked documents** panel. All of this work was documented in **specification** for designers and developers.

## Redesigning the panel system

Working through the existing panels, a few recurring problems stood out:

{% include cards-3-cols.liquid source=site.data.projects.erp-panels.problems %}

I started from the **foundation**: the **anatomy** of the system — the **icon toolbar** as the single entry point, and the **panel** with its consistent structure and elements.

<div class="mx-auto" style="max-width: 520px;">
{% include animated-image.liquid src="https://cdn.jsdelivr.net/gh/nszczerba99/ux-portfolio-images@main/projects/erp-panels/panel-anatomy.webp" alt="The redesigned panel anatomy: the panel with its actions, and the icon toolbar with general and app-specific views." %}
</div>

The toolbar hosts two kinds of views: **general** ones, shared by all applications — like messages, favorites or history — and **app-specific** ones that exist only in a given application, like linked documents in Sales orders. Previously the two were **mixed together** even though they work differently — now they are **clearly separated** on the toolbar.

### Configuration you can find

Configuration now lives where users expect it. Each toolbar has a **settings menu** where users simply **toggle which views are visible**.

**Toolbars layouts** operate on a bigger scale: one layout saves the configuration of **all toolbars**, with general views persisted **across all applications** and app-specific ones **per application**. That's why they live in the **top bar** rather than on a single toolbar — users can save **personal** layouts or share them across the **organization**, switch between them, and manage them in a dedicated modal.

<div class="row g-4 align-items-start">
    <div class="col-md-6 col-12">
      {% include animated-image.liquid src="https://cdn.jsdelivr.net/gh/nszczerba99/ux-portfolio-images@main/projects/erp-panels/visible-views-menu.webp" alt="Toolbar settings with the Visible views submenu, grouped into general and app-specific views." %}
    </div>
    <div class="col-md-6 col-12">
      {% include animated-image.liquid src="https://cdn.jsdelivr.net/gh/nszczerba99/ux-portfolio-images@main/projects/erp-panels/toolbar-layouts-dropdown.webp" alt="The toolbars layout dropdown in the top bar with system, personal and organization layouts." %}
    </div>
</div>

<div class="mx-auto" style="max-width: 640px;">
{% include animated-image.liquid src="https://cdn.jsdelivr.net/gh/nszczerba99/ux-portfolio-images@main/projects/erp-panels/manage-layouts-modal.webp" alt="The Manage toolbars layouts modal with reorderable system, personal and organization layouts." %}
</div>

### Fixing the close button

The clearest example of the old system working against its users was the **X button**. In the current interface, closing a panel didn't just close it — it also **removed the panel's icon from the toolbar**.

{% include animated-image.liquid src="https://cdn.jsdelivr.net/gh/nszczerba99/ux-portfolio-images@main/projects/erp-panels/close-behavior-diagram.webp" alt="Diagram comparing the old and new close behavior: before, X closed the panel and removed its icon; now, X only closes the panel." %}

For users, the feature simply seemed **broken**. Getting it back required digging into toolbar configuration — a task most users never discovered. In the redesigned system, the responsibilities are **separated**: **X only closes** the panel, and removing icons from the toolbar is an **explicit, deliberate action** in toolbar settings.

### Predictable pinning

The **pin** now does exactly one thing: a pinned panel **stays docked**, an unpinned one **hides automatically** — the state is visible at a glance on the panel header, and the toolbar icon **never disappears**.

The pin icon itself changed too, to a **more modern, intuitive one**. Before, the pin simply got **crossed out** on click — ambiguous: is that the **current state** or the **action** a click performs? The redesigned control removes the guesswork by clearly showing the current state.

Power users also got a proper **split panel**: several views open at once, stacked in a single panel. On the toolbar, a split panel is represented by the **icon of its top view**, with a **dots indicator** showing there are more views inside. Before, splitting was only possible when multiple views got **pinned** — their icons disappearing from the toolbar one by one — a very convoluted path. Now splitting is **always available**, and the result saves into **toolbars layouts** like everything else.

<div class="row g-4 justify-content-center">
    <div class="col-md-4 col-6">
      {% include animated-image.liquid src="https://cdn.jsdelivr.net/gh/nszczerba99/ux-portfolio-images@main/projects/erp-panels/pinned-panel.webp" alt="A pinned panel with the pin state clearly shown in the header." %}
    </div>
    <div class="col-md-4 col-6">
      {% include animated-image.liquid src="https://cdn.jsdelivr.net/gh/nszczerba99/ux-portfolio-images@main/projects/erp-panels/split-panel.webp" alt="A split panel with three views stacked in one panel, and the toolbar icon with a dots indicator." %}
    </div>
</div>

## Organizing the data table

Sales orders lists in CEE can return **thousands of results**, and the legacy Sales orders list exposed **a lot of filters at once**, permanently occupying a large part of the screen:

{% include animated-image.liquid src="https://cdn.jsdelivr.net/gh/nszczerba99/ux-portfolio-images@main/projects/erp-panels/legacy-sales-orders.webp" alt="The legacy Sales orders list — a large filter section permanently above the table." %}

The redesigned list had already improved on this: only the **most-used filters** stay visible, and the rest moved into a **More filters** panel.

{% include animated-image.liquid src="https://cdn.jsdelivr.net/gh/nszczerba99/ux-portfolio-images@main/projects/erp-panels/more-filters-panel.webp" alt="The redesigned Sales orders list with the More filters panel open." %}

I took it a step further. **Multi-column sorting** and **grouping** are just as much about organizing the table's data as filters are — so I brought them into the **same panel**, one place for all of it: the **table data organization** panel.

{% include animated-image.liquid src="https://cdn.jsdelivr.net/gh/nszczerba99/ux-portfolio-images@main/projects/erp-panels/more-options-panel.webp" alt="The Table options panel with three tabs: Filters, Groups and Sorting." %}

The panel brings the table's **data organization options** into one predictable place, structured into three tabs:

<strong class="text-themed-purple">Filters:</strong> the full filter set, grouped into **collapsible sections**.

<strong class="text-themed-purple">Groups:</strong> **grouping** of table rows by chosen attributes — a way to turn a flat list of a thousand orders into a structured overview.

<strong class="text-themed-purple">Sorting:</strong> **multi-column sorting**, so users can express rules like *"by status, then by creation date"* instead of being limited to a single column.

<div class="row g-4 justify-content-center">
    <div class="col-md-4 col-sm-6 col-10">
      {% include animated-image.liquid src="https://cdn.jsdelivr.net/gh/nszczerba99/ux-portfolio-images@main/projects/erp-panels/filters-tab-panel.webp" alt="The Filters tab of the Table options panel with collapsible filter sections." %}
    </div>
    <div class="col-md-4 col-sm-6 col-10">
      {% include animated-image.liquid src="https://cdn.jsdelivr.net/gh/nszczerba99/ux-portfolio-images@main/projects/erp-panels/groups-tab-panel.webp" alt="The Groups tab of the Table options panel with two grouping rules." %}
    </div>
    <div class="col-md-4 col-sm-6 col-10">
      {% include animated-image.liquid src="https://cdn.jsdelivr.net/gh/nszczerba99/ux-portfolio-images@main/projects/erp-panels/sorting-tab-panel.webp" alt="The Sorting tab of the Table options panel with two sort rules." %}
    </div>
</div>

In the old version, sorting and grouping were squeezed into **one modal**, opened from the table toolbar. Checking a column on the left added it to the list on the right — as either a **sort** or a **grouping** rule. Switching a rule between **sorting** and **grouping** was hidden behind icon dropdowns in the toolbar. Both functions lived in one list, their state was barely visible, and every change took several clicks on unlabeled icons. Neither **user-friendly** nor **intuitive**:

<div class="mx-auto" style="max-width: 640px;">
{% include animated-image.liquid src="https://cdn.jsdelivr.net/gh/nszczerba99/ux-portfolio-images@main/projects/erp-panels/legacy-grouping-sorting-modal.webp" alt="The legacy Specify grouping and sorting modal with a column list on the left and rules on the right." %}
</div>

In the new panel, each grouping and sorting rule is a separate, **draggable** item. The order of the rules matters — the table is grouped or sorted by the first one, then the next — and users can change it by simply **dragging a rule up or down**. Every rule can be **removed** with a single icon button, and in sorting, the **sort direction** is switched right in the row.

<div class="mx-auto" style="max-width: 300px;">
{% include animated-image.liquid src="https://cdn.jsdelivr.net/gh/nszczerba99/ux-portfolio-images@main/projects/erp-panels/sorting-drag.webp" alt="Dragging a sorting rule to change its order." %}
</div>

## Navigating linked documents

An ERP document never lives alone — a **sales order** produces **deliveries**, **picking orders**, **invoices**, etc. CEE showed this chain in a dedicated panel, called **Voucher references chain** in the old version:

<div class="mx-auto" style="max-width: 320px;">
{% include animated-image.liquid src="https://cdn.jsdelivr.net/gh/nszczerba99/ux-portfolio-images@main/projects/erp-panels/voucher-chain-before.webp" alt="Before: the Voucher references chain panel in the old CEE interface." %}
</div>

Like much of the old interface, it was **old-fashioned** and **unintuitive**. To see the linked documents of a document, the user had to **select it in the list** and then click **refresh inside the panel**:

{% include animated-image.liquid src="https://cdn.jsdelivr.net/gh/nszczerba99/ux-portfolio-images@main/projects/erp-panels/voucher-chain-old-1.webp" alt="Recording: selecting a sales order in the list and clicking refresh in the Voucher references chain panel to load its linked documents." %}

Switching between the linked documents of the **whole document** and those of a **single item** required yet another step — picking the right option from the **refresh split button**. Its icon **didn't communicate its function well**, and the menu options, like *Update order reference chain for line item*, were **long** and **hard to understand**:

{% include animated-image.liquid src="https://cdn.jsdelivr.net/gh/nszczerba99/ux-portfolio-images@main/projects/erp-panels/voucher-chain-old-2.webp" alt="Recording: switching the panel between the whole document and a line item via the refresh split button menu." %}

I redesigned it as the **Linked documents** panel. Now, just **selecting a document or an item** in the list automatically shows its linked documents — no refresh needed. The panel also got a **modern, cleaner UI** in line with the Comarch Design System: every document in the chain became an **easy-to-scan card**, with the currently open document explicitly marked. And when nothing is selected yet, a new **empty state** — missing in the old panel — tells users how to get started:

<div class="row g-4 justify-content-center">
    <div class="col-md-4 col-6">
      {% include animated-image.liquid src="https://cdn.jsdelivr.net/gh/nszczerba99/ux-portfolio-images@main/projects/erp-panels/linked-docs-document.webp" alt="After: the Linked documents panel showing the chain of a sales order as cards, with the current document marked." %}
    </div>
    <div class="col-md-4 col-6">
      {% include animated-image.liquid src="https://cdn.jsdelivr.net/gh/nszczerba99/ux-portfolio-images@main/projects/erp-panels/linked-docs-empty.webp" alt="The Linked documents panel empty state: Nothing selected yet. Select a row in the table to see its linked documents." %}
    </div>
</div>

When an item is selected, the panel header **clearly states** that it shows data for that item — and vice versa for the whole document — so users always know what they're looking at:

{% include animated-image.liquid src="https://cdn.jsdelivr.net/gh/nszczerba99/ux-portfolio-images@main/projects/erp-panels/linked-docs-item.webp" alt="After: a sales order with an item selected, and the Linked documents panel header stating it shows that item's chain." %}

When the panel is **unpinned**, selection doesn't drive it. Instead, a **row action** — *Show linked documents* — opens the panel for that row:

{% include animated-image.liquid src="https://cdn.jsdelivr.net/gh/nszczerba99/ux-portfolio-images@main/projects/erp-panels/linked-docs-row-action.webp" alt="The Show linked documents row action in the Sales orders list." %}

Together, these changes turned the panel from a tool users had to **operate** into one that simply **follows their work**: select a document or an item, and its whole chain is right there.

## Outcomes

The Sales Orders redesign was eventually **dropped**, so my designs **never reached customers**. What remained was a complete, documented design: a consistent set of **rules for the panel system**, two redesigned panels, and a **specification** ready for designers and developers to build from.

Even without a release, the project let me work on real problems of a large, mature product — and design a **system of behaviors**, not just individual screens.

## Lessons learnt

### Density is a feature, not a bug
Working on a system for **professional daily users** taught me to respect **information density**. The goal was never to simplify CEE into a consumer app — it was to make its density **navigable**: predictable panels, clear hierarchy, and progressive disclosure instead of fewer capabilities.

### A specification is a designed product too
The biggest part of this project was not drawing panels — it was **writing the rules**: edge cases like split panels, what a toolbar layout **remembers between sessions**, or how organization-wide layouts propagate to users. I learned to write specs that designers and developers can **quickly understand and act on**.

### Design also means convincing people
The other designer and I were pushing for the redesign while most colleagues were **used to the old system** and skeptical of any changes. A big part of the work was **explaining and defending** our decisions — showing the problems with concrete examples and why the changes were needed. I learned that good design is not enough on its own: you also have to **win people over**.

{% include projects/ai-disclosure.liquid %}
