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

1. Clone our Github repo somewhere in your machine
  ```bash
  $ git clone https://github.com/tetherless-world/nhanes-hadatac.git
  ```

2. Navigate to the docker compose file path
  ```bash
  $ cd nhanes-hadatac/docker/
  ```

3. Start the NHANES-KG services using docker compose up
  ```bash
  $ docker-compose up -d
  ```

4. Point your web browser to [http://localhost:9000](http://localhost:9000) to confirm everything is running as expected. You should see HADatAc's initial dashboard with some numbers about the NHANES-KG.

<small>
In most Linux systems `localhost` will be used. However, in MacOS or Windows hosts you will need to check your environment as the Docker containers might be running virtualized. In these cases, it may be required to know the IP for the virtual machine.
</small>

### First steps: Interacting with NHANES-KG

Follow this [tutorial]({{ site.url }}{% link first-steps.md %}).

### Manual deployment: Deploy NHANES-KG in a fresh HADatAc

An in-depth guide for this will be available soon.

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