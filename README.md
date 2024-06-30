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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C627%20hrs%2038%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1541 commits        ██████░░░░░░░░░░░░░░░░░░░   24.31 % 
🌆 Daytime                2724 commits        ███████████░░░░░░░░░░░░░░   42.98 % 
🌃 Evening                1830 commits        ███████░░░░░░░░░░░░░░░░░░   28.87 % 
🌙 Night                  243 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.83 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   922 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.55 % 
Tuesday                  862 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.60 % 
Wednesday                795 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.54 % 
Thursday                 835 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.17 % 
Friday                   831 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.11 % 
Saturday                 1041 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.42 % 
Sunday                   1052 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.60 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       16 hrs 52 mins      █████████████████░░░░░░░░   68.17 % 
YAML                     5 hrs 50 mins       ██████░░░░░░░░░░░░░░░░░░░   23.62 % 
Docker                   37 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.55 % 
Bash                     28 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.95 % 
Other                    21 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.42 % 

🔥 Editors: 
Zsh                      16 hrs 52 mins      █████████████████░░░░░░░░   68.17 % 
VS Code                  7 hrs 37 mins       ████████░░░░░░░░░░░░░░░░░   30.83 % 
Obsidian                 8 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.59 % 
Vim                      6 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.41 % 

💻 Operating System: 
Linux                    24 hrs 45 mins      █████████████████████████   100.00 % 
```


 Last Updated on 30/06/2024 00:43:17 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
