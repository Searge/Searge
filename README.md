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
🌞 Morning                2046 commits        ██████░░░░░░░░░░░░░░░░░░░   25.97 % 
🌆 Daytime                3441 commits        ███████████░░░░░░░░░░░░░░   43.68 % 
🌃 Evening                2117 commits        ███████░░░░░░░░░░░░░░░░░░   26.88 % 
🌙 Night                  273 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.47 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       11 hrs 23 mins      ███████████░░░░░░░░░░░░░░   42.50 % 
YAML                     6 hrs 45 mins       ██████░░░░░░░░░░░░░░░░░░░   25.21 % 
Markdown                 4 hrs 43 mins       ████░░░░░░░░░░░░░░░░░░░░░   17.61 % 
Terraform                1 hr 12 mins        █░░░░░░░░░░░░░░░░░░░░░░░░   04.52 % 
Python                   44 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.77 % 

🔥 Editors: 
VS Code                  14 hrs 58 mins      ██████████████░░░░░░░░░░░   55.86 % 
Zsh                      11 hrs 23 mins      ███████████░░░░░░░░░░░░░░   42.50 % 
Obsidian                 23 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.49 % 
Vim                      2 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.15 % 

💻 Operating System: 
Linux                    26 hrs 47 mins      █████████████████████████   100.00 % 
```


 Last Updated on 27/07/2025 00:08:11 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
