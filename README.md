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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C720%20hrs%2052%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1586 commits        ██████░░░░░░░░░░░░░░░░░░░   24.41 % 
🌆 Daytime                2828 commits        ███████████░░░░░░░░░░░░░░   43.52 % 
🌃 Evening                1843 commits        ███████░░░░░░░░░░░░░░░░░░   28.36 % 
🌙 Night                  241 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.71 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   987 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.19 % 
Tuesday                  918 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.13 % 
Wednesday                803 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.36 % 
Thursday                 861 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.25 % 
Friday                   849 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.07 % 
Saturday                 1005 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.47 % 
Sunday                   1075 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.54 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       10 hrs 57 mins      ████████████░░░░░░░░░░░░░   49.52 % 
YAML                     7 hrs 51 mins       █████████░░░░░░░░░░░░░░░░   35.48 % 
Markdown                 1 hr 41 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   07.63 % 
Bash                     58 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.43 % 
Docker                   19 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.49 % 

🔥 Editors: 
Zsh                      10 hrs 57 mins      ████████████░░░░░░░░░░░░░   49.52 % 
VS Code                  9 hrs 26 mins       ███████████░░░░░░░░░░░░░░   42.62 % 
Obsidian                 1 hr 35 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   07.18 % 
Vim                      9 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.69 % 

💻 Operating System: 
Linux                    22 hrs 8 mins       █████████████████████████   100.00 % 
```


 Last Updated on 14/08/2024 00:44:53 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
