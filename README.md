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
🌞 Morning                1727 commits        ██████░░░░░░░░░░░░░░░░░░░   25.45 % 
🌆 Daytime                2866 commits        ███████████░░░░░░░░░░░░░░   42.23 % 
🌃 Evening                1935 commits        ███████░░░░░░░░░░░░░░░░░░   28.51 % 
🌙 Night                  258 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.80 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       7 hrs 59 mins       █████████████████░░░░░░░░   69.70 % 
Markdown                 2 hrs 35 mins       ██████░░░░░░░░░░░░░░░░░░░   22.63 % 
Text                     22 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.24 % 
JSON                     13 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.94 % 
YAML                     7 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   01.12 % 

🔥 Editors: 
Zsh                      7 hrs 59 mins       █████████████████░░░░░░░░   69.70 % 
Obsidian                 2 hrs 35 mins       ██████░░░░░░░░░░░░░░░░░░░   22.63 % 
VS Code                  51 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   07.56 % 
Vim                      0 secs              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.12 % 

💻 Operating System: 
Linux                    11 hrs 27 mins      █████████████████████████   100.00 % 
```


 Last Updated on 05/01/2025 00:47:28 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
