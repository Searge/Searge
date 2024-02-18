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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C420%20hrs%2035%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1526 commits        ██████░░░░░░░░░░░░░░░░░░░   22.83 % 
🌆 Daytime                2972 commits        ███████████░░░░░░░░░░░░░░   44.47 % 
🌃 Evening                1952 commits        ███████░░░░░░░░░░░░░░░░░░   29.21 % 
🌙 Night                  233 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.49 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   934 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.98 % 
Tuesday                  831 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.43 % 
Wednesday                889 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.30 % 
Thursday                 937 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.02 % 
Friday                   860 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.87 % 
Saturday                 1005 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.04 % 
Sunday                   1227 commits        █████░░░░░░░░░░░░░░░░░░░░   18.36 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 1 hr 20 mins        ██████████░░░░░░░░░░░░░░░   39.81 % 
Bash                     50 mins             ██████░░░░░░░░░░░░░░░░░░░   24.86 % 
INI                      22 mins             ███░░░░░░░░░░░░░░░░░░░░░░   11.21 % 
YAML                     22 mins             ███░░░░░░░░░░░░░░░░░░░░░░   11.15 % 
Docker                   11 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   05.62 % 

🔥 Editors: 
VS Code                  1 hr 50 mins        ██████████████░░░░░░░░░░░   54.64 % 
Obsidian                 1 hr 8 mins         ████████░░░░░░░░░░░░░░░░░   33.71 % 
Vim                      19 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   09.89 % 
Neovim                   3 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   01.76 % 

💻 Operating System: 
Linux                    3 hrs 22 mins       █████████████████████████   100.00 % 
```


 Last Updated on 18/02/2024 00:10:13 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
