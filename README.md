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
🌞 Morning                1714 commits        ███████░░░░░░░░░░░░░░░░░░   26.02 % 
🌆 Daytime                2803 commits        ███████████░░░░░░░░░░░░░░   42.55 % 
🌃 Evening                1825 commits        ███████░░░░░░░░░░░░░░░░░░   27.71 % 
🌙 Night                  245 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.72 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       9 hrs 11 mins       ██████████████░░░░░░░░░░░   54.56 % 
YAML                     4 hrs 49 mins       ███████░░░░░░░░░░░░░░░░░░   28.60 % 
Markdown                 2 hrs 4 mins        ███░░░░░░░░░░░░░░░░░░░░░░   12.33 % 
INI                      13 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.31 % 
Go                       12 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.21 % 

🔥 Editors: 
Zsh                      9 hrs 11 mins       ██████████████░░░░░░░░░░░   54.56 % 
VS Code                  7 hrs 33 mins       ███████████░░░░░░░░░░░░░░   44.90 % 
Obsidian                 5 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.51 % 
Vim                      0 secs              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.02 % 

💻 Operating System: 
Linux                    16 hrs 50 mins      █████████████████████████   100.00 % 
```


 Last Updated on 09/03/2025 00:52:23 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
