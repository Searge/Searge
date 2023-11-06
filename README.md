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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C310%20hrs%2021%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1486 commits        ██████░░░░░░░░░░░░░░░░░░░   22.52 % 
🌆 Daytime                2965 commits        ███████████░░░░░░░░░░░░░░   44.94 % 
🌃 Evening                1920 commits        ███████░░░░░░░░░░░░░░░░░░   29.10 % 
🌙 Night                  227 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.44 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   963 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.60 % 
Tuesday                  843 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.78 % 
Wednesday                842 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.76 % 
Thursday                 925 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.02 % 
Friday                   850 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.88 % 
Saturday                 983 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.90 % 
Sunday                   1192 commits        █████░░░░░░░░░░░░░░░░░░░░   18.07 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 4 hrs 50 mins       █████████░░░░░░░░░░░░░░░░   37.50 % 
YAML                     3 hrs 58 mins       ████████░░░░░░░░░░░░░░░░░   30.80 % 
Other                    1 hr 14 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   09.60 % 
conf                     48 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   06.24 % 
Jinja2                   35 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.54 % 

🔥 Editors: 
VS Code                  6 hrs 40 mins       █████████████░░░░░░░░░░░░   51.69 % 
Obsidian                 4 hrs 18 mins       ████████░░░░░░░░░░░░░░░░░   33.30 % 
Vim                      1 hr 56 mins        ████░░░░░░░░░░░░░░░░░░░░░   15.01 % 

💻 Operating System: 
Linux                    12 hrs 54 mins      █████████████████████████   100.00 % 
```


 Last Updated on 06/11/2023 00:09:59 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
