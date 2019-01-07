---
name: clients
title:
short-title: Clients
keywords:
meta:
title-banner:
  title: Posting <b class="highlight">all</b> the things.
filters:
  - title: Things We’ve Learned
    category: cat-things-weve-learned
  - title: Team Building
    category: cat-team-building
  - title: What’s Happening
    category: cat-whats-happening 
  - title: Games
    category: cat-games
  - title: View All Posts
    category: cat-all
---
{{#each posts}}
{{#post this}}

{{#if cover}}

{{>column-start classes=categories}}

  {{>link link-post=name h2=true text=short-title}}

  {{>post-overview}}

  {{>quotes}}
  
  {{>link link-post=name text="Read more >"}}

{{>column-end}}

{{>column-start classes=categories}}

  {{>image cover}}

{{>column-end}}

{{>clearfix classes=categories}}

{{else}}

{{>column-start full=true classes=categories}}

  {{>link link-post=name h2=true text=short-title}}

  {{>post-overview}}

  {{>quotes}}
  
  {{>link link-post=name text="Read more >"}}

{{>column-end}}

{{/if}}

{{/post}}
{{/each}}
