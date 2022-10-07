---
layout: default
title: Home
nav_order: 1
description: "This is the official website for all things related to the NHANES Knowledge Graph built by the Tetherless World Constellation at Rensselaer Polytechnic Institute."
---

# NHANES-KG: The National Health and Nutrition Examination Surveys Knowledge Graph
{: .fs-9 }

This is the official website for all things related to the NHANES Knowledge Graph built by the Tetherless World Constellation at Rensselaer Polytechnic Institute.
{: .fs-6 .fw-300 }

[Get started now](#getting-started){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 } [View it on GitHub](https://github.com/tetherless-world/nhanes-hadatac){: .btn .fs-5 .mb-4 .mb-md-0 }

---

## Getting started

### Dependencies

The NHANES-KG is deployed using [HADatAc](http://hadatac.org), a scientific knowledge graph framework. In its turn, HADatAc is more easily deployed using [Docker](http://docker.com). While you are welcome to build the NHANES-KG from scratch using all the [provided data and metadata](https://github.com/tetherless-world/nhanes-hadatac), luckily, we have pre-built Docker images with NHANES-KG for you. Therefore, you'll only need the following to begin:

1. [Docker Engine](https://docs.docker.com/engine/install/)
2. [Docker Compose](https://docs.docker.com/compose/install/)
3. [Git](https://git-scm.com/) - you most likely already have this one.

### Quick start: Run NHANES-HADatAc Docker containers

1. Add Just the Docs to your Jekyll site's `_config.yml` as a [remote theme](https://blog.github.com/2017-11-29-use-any-theme-with-github-pages/)

```yaml
remote_theme: just-the-docs/just-the-docs
```

<small>You must have GitHub Pages enabled on your repo, one or more Markdown files, and a `_config.yml` file. [See an example repository](https://github.com/pmarsceill/jtd-remote)</small>

### Local installation: Use the gem-based theme

1. Install the Ruby Gem
  ```bash
  $ gem install just-the-docs
  ```
  ```yaml
  # .. or add it to your Jekyll site’s Gemfile
  gem "just-the-docs"
  ```

2. Add Just the Docs to your Jekyll site’s `_config.yml`
  ```yaml
  theme: "just-the-docs"
  ```

3. _Optional:_ Initialize search data (creates `search-data.json`)
  ```bash
  $ bundle exec just-the-docs rake search:init
  ```

3. Run your local Jekyll server
  ```bash
  $ jekyll serve
  ```
  ```bash
  # .. or if you're using a Gemfile (bundler)
  $ bundle exec jekyll serve
  ```


4. Point your web browser to [http://localhost:4000](http://localhost:4000)

If you're hosting your site on GitHub Pages, [set up GitHub Pages and Jekyll locally](https://help.github.com/en/articles/setting-up-your-github-pages-site-locally-with-jekyll) so that you can more easily work in your development environment.

### Configure Just the Docs

- [See configuration options]({{ site.baseurl }})

---

## About the project

Just the Docs is &copy; 2017-{{ "now" | date: "%Y" }} by [Patrick Marsceill](http://patrickmarsceill.com).

### License

Just the Docs is distributed by an [MIT license](https://github.com/just-the-docs/just-the-docs/tree/main/LICENSE.txt).

### Contributing

When contributing to this repository, please first discuss the change you wish to make via issue,
email, or any other method with the owners of this repository before making a change. Read more about becoming a contributor in [our GitHub repo](https://github.com/just-the-docs/just-the-docs#contributing).

#### Thank you to the contributors of Just the Docs!

<ul class="list-style-none">
{% for contributor in site.github.contributors %}
  <li class="d-inline-block mr-1">
     <a href="{{ contributor.html_url }}"><img src="{{ contributor.avatar_url }}" width="32" height="32" alt="{{ contributor.login }}"/></a>
  </li>
{% endfor %}
</ul>

### Code of Conduct

Just the Docs is committed to fostering a welcoming community.

[View our Code of Conduct](https://github.com/just-the-docs/just-the-docs/tree/main/CODE_OF_CONDUCT.md) on our GitHub repository.