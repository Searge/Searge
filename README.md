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
🌞 Morning                1955 commits        ███████░░░░░░░░░░░░░░░░░░   26.22 % 
🌆 Daytime                3178 commits        ███████████░░░░░░░░░░░░░░   42.63 % 
🌃 Evening                2052 commits        ███████░░░░░░░░░░░░░░░░░░   27.53 % 
🌙 Night                  270 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.62 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
YAML                     9 hrs 42 mins       ██████████░░░░░░░░░░░░░░░   39.52 % 
sh                       7 hrs 12 mins       ███████░░░░░░░░░░░░░░░░░░   29.36 % 
Markdown                 4 hrs 5 mins        ████░░░░░░░░░░░░░░░░░░░░░   16.63 % 
JSON                     1 hr 43 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   07.01 % 
Bash                     42 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.86 % 

🔥 Editors: 
VS Code                  12 hrs 29 mins      █████████████░░░░░░░░░░░░   50.88 % 
Zsh                      7 hrs 12 mins       ███████░░░░░░░░░░░░░░░░░░   29.36 % 
Obsidian                 2 hrs 49 mins       ███░░░░░░░░░░░░░░░░░░░░░░   11.52 % 
Cursor                   2 hrs 1 min         ██░░░░░░░░░░░░░░░░░░░░░░░   08.23 % 

💻 Operating System: 
Linux                    24 hrs 33 mins      █████████████████████████   100.00 % 
```


 Last Updated on 06/07/2025 00:07:45 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
