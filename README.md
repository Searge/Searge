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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C788%20hrs%2010%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1668 commits        ██████░░░░░░░░░░░░░░░░░░░   25.20 % 
🌆 Daytime                2842 commits        ███████████░░░░░░░░░░░░░░   42.94 % 
🌃 Evening                1861 commits        ███████░░░░░░░░░░░░░░░░░░   28.12 % 
🌙 Night                  248 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.75 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   974 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.72 % 
Tuesday                  937 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.16 % 
Wednesday                847 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.80 % 
Thursday                 884 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.36 % 
Friday                   880 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.30 % 
Saturday                 1026 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.50 % 
Sunday                   1071 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.18 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       8 hrs 12 mins       ██████████████░░░░░░░░░░░   54.46 % 
YAML                     5 hrs 22 mins       █████████░░░░░░░░░░░░░░░░   35.63 % 
Other                    1 hr 2 mins         ██░░░░░░░░░░░░░░░░░░░░░░░   06.90 % 
DNS Zone                 12 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.35 % 
Markdown                 6 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.67 % 

🔥 Editors: 
Zsh                      8 hrs 12 mins       ██████████████░░░░░░░░░░░   54.46 % 
VS Code                  6 hrs 43 mins       ███████████░░░░░░░░░░░░░░   44.62 % 
Obsidian                 6 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.67 % 
Vim                      2 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.25 % 

💻 Operating System: 
Linux                    15 hrs 4 mins       █████████████████████████   100.00 % 
```


 Last Updated on 26/09/2024 00:47:54 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
