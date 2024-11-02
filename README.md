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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C892%20hrs%2013%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1924 commits        ██████░░░░░░░░░░░░░░░░░░░   25.86 % 
🌆 Daytime                2933 commits        ██████████░░░░░░░░░░░░░░░   39.42 % 
🌃 Evening                2286 commits        ████████░░░░░░░░░░░░░░░░░   30.72 % 
🌙 Night                  298 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   04.00 % 
```
📅 **I'm Most Productive on Saturday** 

```text
Monday                   1010 commits        ███░░░░░░░░░░░░░░░░░░░░░░   13.57 % 
Tuesday                  920 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.36 % 
Wednesday                935 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.57 % 
Thursday                 923 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.40 % 
Friday                   900 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.10 % 
Saturday                 1407 commits        █████░░░░░░░░░░░░░░░░░░░░   18.91 % 
Sunday                   1346 commits        █████░░░░░░░░░░░░░░░░░░░░   18.09 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       9 hrs 32 mins       █████████████░░░░░░░░░░░░   51.00 % 
YAML                     5 hrs 48 mins       ████████░░░░░░░░░░░░░░░░░   31.04 % 
Other                    1 hr 21 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   07.31 % 
Markdown                 22 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.02 % 
Git Config               19 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.78 % 

🔥 Editors: 
Zsh                      9 hrs 32 mins       █████████████░░░░░░░░░░░░   51.00 % 
VS Code                  5 hrs 43 mins       ████████░░░░░░░░░░░░░░░░░   30.63 % 
Cursor                   2 hrs 49 mins       ████░░░░░░░░░░░░░░░░░░░░░   15.14 % 
Vim                      21 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.90 % 
Obsidian                 14 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.33 % 

💻 Operating System: 
Linux                    18 hrs 42 mins      █████████████████████████   100.00 % 
```


 Last Updated on 02/11/2024 00:49:31 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
