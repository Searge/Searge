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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C174%20hrs%2036%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1279 commits        ██████░░░░░░░░░░░░░░░░░░░   22.76 % 
🌆 Daytime                2535 commits        ███████████░░░░░░░░░░░░░░   45.11 % 
🌃 Evening                1585 commits        ███████░░░░░░░░░░░░░░░░░░   28.20 % 
🌙 Night                  221 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.93 % 
```
📅 **I'm Most Productive on Saturday** 

```text
Monday                   796 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.16 % 
Tuesday                  746 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.27 % 
Wednesday                750 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.35 % 
Thursday                 797 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.18 % 
Friday                   805 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.32 % 
Saturday                 863 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.36 % 
Sunday                   863 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.36 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 2 hrs 1 min         ███████████████████████░░   93.53 % 
YAML                     4 mins              █░░░░░░░░░░░░░░░░░░░░░░░░   03.80 % 
Bash                     3 mins              █░░░░░░░░░░░░░░░░░░░░░░░░   02.38 % 
Other                    0 secs              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.19 % 
JSON                     0 secs              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.07 % 

🔥 Editors: 
Obsidian                 1 hr 46 mins        █████████████████████░░░░   82.54 % 
VS Code                  22 mins             ████░░░░░░░░░░░░░░░░░░░░░   17.46 % 

💻 Operating System: 
Windows                  1 hr 44 mins        ████████████████████░░░░░   80.66 % 
Linux                    25 mins             █████░░░░░░░░░░░░░░░░░░░░   19.34 % 
```


 Last Updated on 13/08/2023 00:09:24 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
