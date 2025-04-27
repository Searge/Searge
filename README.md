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
🌞 Morning                1859 commits        ███████░░░░░░░░░░░░░░░░░░   26.06 % 
🌆 Daytime                3009 commits        ███████████░░░░░░░░░░░░░░   42.18 % 
🌃 Evening                2008 commits        ███████░░░░░░░░░░░░░░░░░░   28.15 % 
🌙 Night                  257 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.60 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       12 hrs 51 mins      ███████████░░░░░░░░░░░░░░   43.57 % 
Terraform                9 hrs 24 mins       ████████░░░░░░░░░░░░░░░░░   31.89 % 
JSON                     4 hrs 11 mins       ████░░░░░░░░░░░░░░░░░░░░░   14.18 % 
HCL                      1 hr 16 mins        █░░░░░░░░░░░░░░░░░░░░░░░░   04.32 % 
Markdown                 58 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.28 % 

🔥 Editors: 
VS Code                  16 hrs 20 mins      ██████████████░░░░░░░░░░░   55.33 % 
Zsh                      12 hrs 51 mins      ███████████░░░░░░░░░░░░░░   43.57 % 
Vim                      11 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   00.67 % 
Obsidian                 3 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.22 % 
Sublime Text             3 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.21 % 

💻 Operating System: 
Linux                    29 hrs 31 mins      █████████████████████████   100.00 % 
```


 Last Updated on 27/04/2025 00:07:34 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
