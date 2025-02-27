---
title: About
permalink: /about
layout: main
---

{{site.title}} is built as a Jekyll static site, from the GitHub repo [{{site.repository}}]({{site.repository}}).

# Who is this for?

This webring is for any natal women on the internet with normie woman blogs :) 

## Requirements

- Either
  - Email me at [zucch1n1@posteo.net](mailto://zucch1n1@posteo.net) with the URL, Site Name, and Description
  - Create a Pull Request on the [Github Repo]({{ site.new_site_url }}) using the below instructions
- Add the iframe to your site / profile
- Not having the iframe on the main page of your site or profile means that you could be removed from the ring.

## Add the iframe to your site

Each member site gets an embed page generated for them. After your pull request is approved and merged, add the embed to your site with the markup:

```
<style type="text/css">
  iframe {
    border: none;
  }
</style>
<iframe src="{{'https://beefsteaktomatoes.github.io/normie-woman-ring/sites/yarnandpeeps.html' | absolute_url}}">
</iframe>
<script src="{{'https://beefsteaktomatoes.github.io/normie-woman-ring/assets/parent.js' | absolute_url }}"></script>
```

replacing `yarnandpeeps` with the name of the file you added. The `parent.js` script is unnecessary if you plan to size the iframe appropriately. It'll look like this:


<style type="text/css">
  iframe {
    border: none;
  }
</style>
<iframe src="{{'https://beefsteaktomatoes.github.io/normie-woman-ring/sites/yarnandpeeps.html' | absolute_url}}">
</iframe>
<script src="{{'https://beefsteaktomatoes.github.io/normie-woman-ring/assets/parent.js' | absolute_url }}"></script>
## Creating a PR

Visit the [create new file form]({{site.new_site_url}}) on this webring's repository.

Name your new file uniquely, and give it an extension of `.html`. Add some [Jekyll front matter](https://jekyllrb.com/docs/front-matter/) along the lines of the following:

```
---
uri: https://yarn-and-peeps.neocities.org/
title: Yarn and Peeps
desc: Knitting, chickens, motherhood, cloth diapers, zero waste
date: 2025-02-21
---
```

where `date` is the day you're making the new file request. Be careful not to mistake `uri` for `url`.

# Custom CSS

If lavender isn't your thing, use your own css by appending the `stylesheet` query string param to the iframe's src attribute.

```
<style type="text/css">
  iframe {
    border: none;
  }
</style>
<iframe src="{{'https://beefsteaktomatoes.github.io/normie-woman-ring/sites/yarnandpeeps.html' | absolute_url}}?stylesheet=<link to your custom stylesheet>">
</iframe>
<script src="{{'https://beefsteaktomatoes.github.io/normie-woman-ring/assets/parent.js' | absolute_url}}"></script>
```

# Manual Implementations

The list of all member sites is available in JSON at the page [sites.json]({{"/sites.json" | absolute_url}}), for sites that would rather construct their embeds themselves.
