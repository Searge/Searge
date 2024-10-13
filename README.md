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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C831%20hrs%2051%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1638 commits        ██████░░░░░░░░░░░░░░░░░░░   25.13 % 
🌆 Daytime                2794 commits        ███████████░░░░░░░░░░░░░░   42.87 % 
🌃 Evening                1837 commits        ███████░░░░░░░░░░░░░░░░░░   28.19 % 
🌙 Night                  248 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.81 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   938 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.39 % 
Tuesday                  893 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.70 % 
Wednesday                853 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.09 % 
Thursday                 874 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.41 % 
Friday                   874 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.41 % 
Saturday                 1014 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.56 % 
Sunday                   1071 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.43 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       10 hrs 7 mins       ██████████████░░░░░░░░░░░   54.68 % 
YAML                     6 hrs 54 mins       █████████░░░░░░░░░░░░░░░░   37.32 % 
Markdown                 37 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.40 % 
Other                    23 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.16 % 
Bash                     11 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.02 % 

🔥 Editors: 
Zsh                      10 hrs 7 mins       ██████████████░░░░░░░░░░░   54.68 % 
VS Code                  7 hrs 46 mins       ███████████░░░░░░░░░░░░░░   42.04 % 
Obsidian                 23 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.14 % 
Vim                      12 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.13 % 

💻 Operating System: 
Linux                    18 hrs 30 mins      █████████████████████████   100.00 % 
```


 Last Updated on 13/10/2024 00:48:25 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
