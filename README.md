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
🌞 Morning                1878 commits        ██████░░░░░░░░░░░░░░░░░░░   25.96 % 
🌆 Daytime                3035 commits        ██████████░░░░░░░░░░░░░░░   41.95 % 
🌃 Evening                2065 commits        ███████░░░░░░░░░░░░░░░░░░   28.54 % 
🌙 Night                  257 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.55 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       11 hrs 1 min        █████████░░░░░░░░░░░░░░░░   35.94 % 
YAML                     5 hrs 15 mins       ████░░░░░░░░░░░░░░░░░░░░░   17.15 % 
Other                    4 hrs 36 mins       ████░░░░░░░░░░░░░░░░░░░░░   15.05 % 
Terraform                2 hrs 12 mins       ██░░░░░░░░░░░░░░░░░░░░░░░   07.18 % 
HCL                      2 hrs 1 min         ██░░░░░░░░░░░░░░░░░░░░░░░   06.58 % 

🔥 Editors: 
VS Code                  19 hrs 18 mins      ████████████████░░░░░░░░░   62.96 % 
Zsh                      11 hrs 1 min        █████████░░░░░░░░░░░░░░░░   35.94 % 
Obsidian                 17 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   00.94 % 
Vim                      2 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.16 % 

💻 Operating System: 
Linux                    30 hrs 40 mins      █████████████████████████   100.00 % 
```


 Last Updated on 11/05/2025 00:08:04 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
