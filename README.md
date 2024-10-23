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
🌞 Morning                1644 commits        ██████░░░░░░░░░░░░░░░░░░░   25.25 % 
🌆 Daytime                2780 commits        ███████████░░░░░░░░░░░░░░   42.70 % 
🌃 Evening                1838 commits        ███████░░░░░░░░░░░░░░░░░░   28.23 % 
🌙 Night                  248 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.81 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   930 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.29 % 
Tuesday                  881 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.53 % 
Wednesday                862 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.24 % 
Thursday                 871 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.38 % 
Friday                   876 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.46 % 
Saturday                 1014 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.58 % 
Sunday                   1076 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.53 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       12 hrs 23 mins      ██████████████░░░░░░░░░░░   57.51 % 
YAML                     5 hrs 45 mins       ███████░░░░░░░░░░░░░░░░░░   26.76 % 
Markdown                 1 hr 45 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   08.18 % 
Bash                     1 hr                █░░░░░░░░░░░░░░░░░░░░░░░░   04.70 % 
Elixir                   10 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   00.85 % 

🔥 Editors: 
Zsh                      12 hrs 23 mins      ██████████████░░░░░░░░░░░   57.51 % 
VS Code                  7 hrs 56 mins       █████████░░░░░░░░░░░░░░░░   36.85 % 
Obsidian                 57 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.44 % 
Vim                      9 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.76 % 
Cursor                   5 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.43 % 

💻 Operating System: 
Linux                    21 hrs 32 mins      █████████████████████████   100.00 % 
```


 Last Updated on 23/10/2024 00:52:23 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
