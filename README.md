# Hi, I'm Searge <img src="images/vulcan.webp" style="display: inline-block; margin: 0; height: 2rem" alt="Vulcan salute" />

## DevOps Engineer at [Smile Ukraine](https://smile-ukraine.com/en)

[![Stand With Ukraine](https://raw.githubusercontent.com/vshymanskyy/StandWithUkraine/main/badges/StandWithUkraine.svg)](https://stand-with-ukraine.pp.ua)
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

### Statistics

[Skyline for 2021](https://skyline.github.com/Searge/2021)

![Visitors](https://komarev.com/ghpvc/?username=searge&label=Profile%20views&color=0e75b6&style=flat) 
<!--START_SECTION:waka-->
**I'm an Early 🐤** 

```text
🌞 Morning                1959 commits        ███████░░░░░░░░░░░░░░░░░░   26.13 % 
🌆 Daytime                3200 commits        ███████████░░░░░░░░░░░░░░   42.68 % 
🌃 Evening                2074 commits        ███████░░░░░░░░░░░░░░░░░░   27.66 % 
🌙 Night                  264 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.52 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       6 hrs 20 mins       ███████████░░░░░░░░░░░░░░   44.23 % 
YAML                     3 hrs 39 mins       ██████░░░░░░░░░░░░░░░░░░░   25.45 % 
Markdown                 1 hr 34 mins        ███░░░░░░░░░░░░░░░░░░░░░░   10.93 % 
Docker                   33 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.93 % 
Other                    28 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.34 % 

🔥 Editors: 
VS Code                  7 hrs 37 mins       █████████████░░░░░░░░░░░░   53.08 % 
Zsh                      6 hrs 20 mins       ███████████░░░░░░░░░░░░░░   44.23 % 
Obsidian                 23 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.69 % 

💻 Operating System: 
Linux                    14 hrs 21 mins      █████████████████████████   100.00 % 
```


 Last Updated on 03/08/2025 00:08:21 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
