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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C147%20hrs%201%20min-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1208 commits        ██████░░░░░░░░░░░░░░░░░░░   22.40 % 
🌆 Daytime                2429 commits        ███████████░░░░░░░░░░░░░░   45.04 % 
🌃 Evening                1547 commits        ███████░░░░░░░░░░░░░░░░░░   28.69 % 
🌙 Night                  209 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.88 % 
```
📅 **I'm Most Productive on Saturday** 

```text
Monday                   776 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.39 % 
Tuesday                  723 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.41 % 
Wednesday                697 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.92 % 
Thursday                 767 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.22 % 
Friday                   777 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.41 % 
Saturday                 834 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.46 % 
Sunday                   819 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.19 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 3 hrs 10 mins       ████████████░░░░░░░░░░░░░   46.00 % 
YAML                     1 hr 18 mins        █████░░░░░░░░░░░░░░░░░░░░   18.96 % 
Other                    56 mins             ███░░░░░░░░░░░░░░░░░░░░░░   13.65 % 
Bash                     40 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   09.69 % 
INI                      25 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   06.18 % 

🔥 Editors: 
VS Code                  3 hrs 38 mins       █████████████░░░░░░░░░░░░   52.93 % 
Obsidian                 3 hrs 1 min         ███████████░░░░░░░░░░░░░░   44.02 % 
Vim                      12 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.05 % 

💻 Operating System: 
Linux                    6 hrs 53 mins       █████████████████████████   100.00 % 
```


 Last Updated on 19/07/2023 00:12:33 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
