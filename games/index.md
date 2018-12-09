---
name: games
title:
keywords:
meta:
title-banner:
  title: <b class="highlight">Games</b> for every team challenge.
filters:
  - title: Communication
    category: cat-communication
  - title: Trust
    category: cat-trust
  - title: Innovation
    category: cat-innovation
  - title: Conflict Resolution
    category: cat-conflict-resolution
  - title: Empathy
    category: cat-empathy
  - title: Productivity
    category: cat-productivity
  - title: Leadership
    category: cat-leadership
  - title: Focus
    category: cat-focus
  - title: Something Different
    category: cat-something-different-games 
  - title: View All Games
    category: cat-all
---
{{#each games}}
{{#game this}}

{{>column-start classes=categories}}

  {{>link link-game=name h2=true text=short-title}}
  
  {{>game-overview}}

  {{>quotes}}

  {{>link link-game=name text="Read more >"}}

{{>column-end}}

{{>column-start classes=categories}}

  {{>video}}

{{>column-end}}

{{>clearfix classes=categories}}

{{/game}}
{{/each}}