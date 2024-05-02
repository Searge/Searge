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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C459%20hrs%2058%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1498 commits        ██████░░░░░░░░░░░░░░░░░░░   24.15 % 
🌆 Daytime                2699 commits        ███████████░░░░░░░░░░░░░░   43.52 % 
🌃 Evening                1760 commits        ███████░░░░░░░░░░░░░░░░░░   28.38 % 
🌙 Night                  245 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.95 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   885 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.27 % 
Tuesday                  811 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.08 % 
Wednesday                833 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.43 % 
Thursday                 840 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.54 % 
Friday                   847 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.66 % 
Saturday                 980 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.80 % 
Sunday                   1006 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.22 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 2 hrs 30 mins       ██████████████░░░░░░░░░░░   55.02 % 
YAML                     1 hr 42 mins        █████████░░░░░░░░░░░░░░░░   37.62 % 
Other                    13 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   05.03 % 
Bash                     6 mins              █░░░░░░░░░░░░░░░░░░░░░░░░   02.32 % 

🔥 Editors: 
VS Code                  2 hrs 49 mins       ███████████████░░░░░░░░░░   61.99 % 
Obsidian                 1 hr 35 mins        █████████░░░░░░░░░░░░░░░░   35.07 % 
Vim                      8 mins              █░░░░░░░░░░░░░░░░░░░░░░░░   02.94 % 

💻 Operating System: 
Linux                    4 hrs 33 mins       █████████████████████████   100.00 % 
```


 Last Updated on 02/05/2024 00:41:06 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
