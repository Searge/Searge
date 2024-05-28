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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C535%20hrs%2010%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1504 commits        ██████░░░░░░░░░░░░░░░░░░░   24.27 % 
🌆 Daytime                2692 commits        ███████████░░░░░░░░░░░░░░   43.45 % 
🌃 Evening                1760 commits        ███████░░░░░░░░░░░░░░░░░░   28.41 % 
🌙 Night                  240 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.87 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   899 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.51 % 
Tuesday                  838 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.52 % 
Wednesday                800 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.91 % 
Thursday                 827 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.35 % 
Friday                   833 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.44 % 
Saturday                 980 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.82 % 
Sunday                   1019 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.45 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       13 hrs 34 mins      ██████████████░░░░░░░░░░░   56.42 % 
YAML                     8 hrs 31 mins       █████████░░░░░░░░░░░░░░░░   35.46 % 
Markdown                 1 hr 26 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   06.00 % 
Other                    20 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.40 % 
Python                   6 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.44 % 

🔥 Editors: 
Zsh                      13 hrs 34 mins      ██████████████░░░░░░░░░░░   56.42 % 
VS Code                  9 hrs 14 mins       ██████████░░░░░░░░░░░░░░░   38.46 % 
Obsidian                 1 hr 8 mins         █░░░░░░░░░░░░░░░░░░░░░░░░   04.74 % 
Vim                      5 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.38 % 

💻 Operating System: 
Linux                    23 hrs 56 mins      █████████████████████████   99.56 % 
Windows                  6 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.44 % 
```


 Last Updated on 28/05/2024 00:41:31 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
