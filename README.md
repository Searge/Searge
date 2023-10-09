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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C263%20hrs%2014%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1410 commits        ██████░░░░░░░░░░░░░░░░░░░   22.57 % 
🌆 Daytime                2812 commits        ███████████░░░░░░░░░░░░░░   45.01 % 
🌃 Evening                1799 commits        ███████░░░░░░░░░░░░░░░░░░   28.79 % 
🌙 Night                  227 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.63 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   907 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.52 % 
Tuesday                  801 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.82 % 
Wednesday                814 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.03 % 
Thursday                 880 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.08 % 
Friday                   820 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.12 % 
Saturday                 947 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.16 % 
Sunday                   1079 commits        ████░░░░░░░░░░░░░░░░░░░░░   17.27 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 10 hrs 8 mins       ██████████████░░░░░░░░░░░   54.09 % 
YAML                     5 hrs 4 mins        ███████░░░░░░░░░░░░░░░░░░   27.05 % 
Docker                   1 hr 1 min          █░░░░░░░░░░░░░░░░░░░░░░░░   05.49 % 
Bash                     28 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.54 % 
Ezhil                    24 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.21 % 

🔥 Editors: 
VS Code                  10 hrs 10 mins      ██████████████░░░░░░░░░░░   54.29 % 
Obsidian                 8 hrs 32 mins       ███████████░░░░░░░░░░░░░░   45.58 % 
Neovim                   1 min               ░░░░░░░░░░░░░░░░░░░░░░░░░   00.13 % 

💻 Operating System: 
Linux                    18 hrs 45 mins      █████████████████████████   100.00 % 
```


 Last Updated on 09/10/2023 00:09:49 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
