---
name: clients
title:
short-title: Clients
keywords:
meta:
title-banner:
  title: Igniting culture in <b class="highlight">every</b> team.
filters:
  - title: Non-profit
    category: cat-non-profit
  - title: Corporate
    category: cat-corporate
  - title: Education
    category: cat-education
  - title: Government
    category: cat-government
  - title: Something Different
    category: cat-something-different-clients 
  - title: View All Clients
    category: cat-all
---
{{#each clients}}
{{#client this}}

{{#if gallery}}

{{>column-start classes=categories}}

  {{>link link-client=name h2=true text=short-title}}

  {{>client-overview}}

  {{>quotes}}
  
  {{>link link-client=name text="Read more >"}}

{{>column-end}}

{{>column-start classes=categories}}

  {{>gallery}}

{{>column-end}}

{{>clearfix classes=categories}}

{{else if video}}

{{>column-start classes=categories}}

  ## {{short-title}}

  {{>client-overview}}

  {{>quotes}}
  
  {{>link link-client=name text="Read more >"}}

{{>column-end}}

{{>column-start classes=categories}}

  {{>video}}

{{>column-end}}

{{>clearfix classes=categories}}

{{else}}

{{>column-start full=true classes=categories}}

  ## {{short-title}}

  {{>client-overview}}

  {{>quotes}}
  
  {{>link link-client=name text="Read more >"}}

{{>column-end}}

{{/if}}

{{/client}}

{{/each}}
