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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C755%20hrs%2021%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1785 commits        ██████░░░░░░░░░░░░░░░░░░░   25.25 % 
🌆 Daytime                2927 commits        ██████████░░░░░░░░░░░░░░░   41.41 % 
🌃 Evening                2085 commits        ███████░░░░░░░░░░░░░░░░░░   29.49 % 
🌙 Night                  272 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.85 % 
```
📅 **I'm Most Productive on Saturday** 

```text
Monday                   1025 commits        ████░░░░░░░░░░░░░░░░░░░░░   14.50 % 
Tuesday                  956 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.52 % 
Wednesday                885 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.52 % 
Thursday                 914 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.93 % 
Friday                   873 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.35 % 
Saturday                 1219 commits        ████░░░░░░░░░░░░░░░░░░░░░   17.24 % 
Sunday                   1197 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.93 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       5 hrs 26 mins       ████████████░░░░░░░░░░░░░   47.99 % 
YAML                     4 hrs 11 mins       █████████░░░░░░░░░░░░░░░░   36.90 % 
Markdown                 38 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   05.66 % 
Terraform                26 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.84 % 
Other                    19 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.93 % 

🔥 Editors: 
Zsh                      5 hrs 26 mins       ████████████░░░░░░░░░░░░░   47.99 % 
VS Code                  5 hrs 2 mins        ███████████░░░░░░░░░░░░░░   44.50 % 
Obsidian                 33 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.87 % 
Vim                      17 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.63 % 

💻 Operating System: 
Linux                    11 hrs 20 mins      █████████████████████████   100.00 % 
```


 Last Updated on 13/09/2024 00:47:22 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
