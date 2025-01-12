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
🌞 Morning                1747 commits        ██████░░░░░░░░░░░░░░░░░░░   25.60 % 
🌆 Daytime                2879 commits        ███████████░░░░░░░░░░░░░░   42.20 % 
🌃 Evening                1939 commits        ███████░░░░░░░░░░░░░░░░░░   28.42 % 
🌙 Night                  258 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.78 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       5 hrs 1 min         ██████████████░░░░░░░░░░░   55.67 % 
Other                    1 hr 49 mins        █████░░░░░░░░░░░░░░░░░░░░   20.15 % 
YAML                     1 hr 8 mins         ███░░░░░░░░░░░░░░░░░░░░░░   12.72 % 
Markdown                 52 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   09.61 % 
Git Config               5 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   01.05 % 

🔥 Editors: 
Zsh                      5 hrs 1 min         ██████████████░░░░░░░░░░░   55.67 % 
VS Code                  3 hrs 11 mins       █████████░░░░░░░░░░░░░░░░   35.31 % 
Obsidian                 48 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   09.01 % 

💻 Operating System: 
Linux                    7 hrs 14 mins       ████████████████████░░░░░   80.19 % 
Windows                  1 hr 47 mins        █████░░░░░░░░░░░░░░░░░░░░   19.81 % 
```


 Last Updated on 12/01/2025 00:44:35 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
