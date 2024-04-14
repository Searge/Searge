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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C453%20hrs%2015%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1416 commits        ██████░░░░░░░░░░░░░░░░░░░   23.72 % 
🌆 Daytime                2645 commits        ███████████░░░░░░░░░░░░░░   44.31 % 
🌃 Evening                1671 commits        ███████░░░░░░░░░░░░░░░░░░   27.99 % 
🌙 Night                  237 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.97 % 
```
📅 **I'm Most Productive on Saturday** 

```text
Monday                   853 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.29 % 
Tuesday                  792 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.27 % 
Wednesday                805 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.49 % 
Thursday                 828 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.87 % 
Friday                   835 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.99 % 
Saturday                 936 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.68 % 
Sunday                   920 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.41 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 2 hrs 42 mins       █████████████████░░░░░░░░   67.47 % 
Other                    35 mins             ████░░░░░░░░░░░░░░░░░░░░░   14.55 % 
Bash                     17 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   07.17 % 
XML                      11 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.66 % 
Lua                      8 mins              █░░░░░░░░░░░░░░░░░░░░░░░░   03.52 % 

🔥 Editors: 
VS Code                  2 hrs 11 mins       ██████████████░░░░░░░░░░░   54.76 % 
Obsidian                 1 hr 45 mins        ███████████░░░░░░░░░░░░░░   43.97 % 
Vim                      3 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   01.26 % 

💻 Operating System: 
Linux                    4 hrs               █████████████████████████   100.00 % 
```


 Last Updated on 14/04/2024 00:38:48 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
