# Hi, I'm Searge <img src="img/vulcan.webp" style="display: inline-block; margin: 0; height: 2rem" alt="Vulcan salute" />

## An DevOps Engineer at [Smile Ukraine](https://smile-ukraine.com/en)

![Visitors](https://komarev.com/ghpvc/?username=searge&label=Profile%20views&color=0e75b6&style=flat) [![Stand With Ukraine](https://raw.githubusercontent.com/vshymanskyy/StandWithUkraine/main/badges/StandWithUkraine.svg)](https://stand-with-ukraine.pp.ua)
<a rel="me" href="https://hachyderm.io/@Searge">![@Searge@hachyderm.io](https://img.shields.io/badge/-@Searge-%232B90D9?logo=mastodon&logoColor=white)</a>

```python
# %%
"""Creating a class for keeping track of knowledge."""
import json
from dataclasses import asdict, make_dataclass

from rich import print

person = make_dataclass(
    "Person",
    [
        ("nick", str),
        ("name", str),
        ("pipelines", list[str]),
        ("web_services", list[str]),
        ("languages", list[str]),
        ("databases", list[str]),
        ("misc", list[str]),
        ("ongoing", list[str]),
    ],
    namespace={"to_json": lambda self: json.dumps(asdict(self), indent=4)},
)

# %%
# @title Initializing classes and creating lists
if __name__ == "__main__":
    pipelines    = ['GitLab Ci', 'GitHub Actions', 'AWS CodePipeline', 'Jenkins']
    web_services = ['nginx', 'apache', 'varnish', 'fastly', 'elastic', 'solr']
    languages    = ['YAML', 'Bash', 'Python', 'JS', 'Web']
    databases    = ['SQLite', 'PostgreSQL', 'Percona', 'DynamoDB', 'Redis']
    misc         = ['Ansible', 'Linux', 'LXC', 'Docker', 'Terraform', 'AWS']
    ongoing      = ['LPIC', 'Full Stack Web', 'AWS']

    me = person('@Searge', 'Sergij Boremchuk',
                pipelines, web_services, languages, databases, misc, ongoing)

    print(me.to_json())

# %%

```

<sub>Thanks @rednafi for idea of script :wink:</sub>

[Skyline for 2021](https://skyline.github.com/Searge/2021)

<!--START_SECTION:waka-->
**I Mostly Code in HTML** 

```text
HTML                     12 repos            ██████░░░░░░░░░░░░░░░░░░░   25.0% 
Python                   7 repos             ███░░░░░░░░░░░░░░░░░░░░░░   14.58% 
JavaScript               6 repos             ███░░░░░░░░░░░░░░░░░░░░░░   12.5% 
Jupyter Notebook         4 repos             ██░░░░░░░░░░░░░░░░░░░░░░░   8.33% 
SCSS                     3 repos             █░░░░░░░░░░░░░░░░░░░░░░░░   6.25%

```


**Timeline**

![Chart not found](https://raw.githubusercontent.com/Searge/Searge/main/charts/bar_graph.png) 


 Last Updated on 24/09/2022 00:24:06 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
