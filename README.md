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
🌞 Morning                1486 commits        ██████░░░░░░░░░░░░░░░░░░░   22.53 % 
🌆 Daytime                2964 commits        ███████████░░░░░░░░░░░░░░   44.93 % 
🌃 Evening                1919 commits        ███████░░░░░░░░░░░░░░░░░░   29.09 % 
🌙 Night                  228 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.46 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   965 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.63 % 
Tuesday                  843 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.78 % 
Wednesday                842 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.76 % 
Thursday                 925 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.02 % 
Friday                   850 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.88 % 
Saturday                 983 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.90 % 
Sunday                   1189 commits        █████░░░░░░░░░░░░░░░░░░░░   18.02 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 4 hrs 23 mins       █████████░░░░░░░░░░░░░░░░   37.10 % 
YAML                     3 hrs 22 mins       ███████░░░░░░░░░░░░░░░░░░   28.43 % 
Other                    1 hr 14 mins        ███░░░░░░░░░░░░░░░░░░░░░░   10.46 % 
conf                     48 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   06.80 % 
Jinja2                   35 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.95 % 

🔥 Editors: 
VS Code                  6 hrs 4 mins        █████████████░░░░░░░░░░░░   51.18 % 
Obsidian                 3 hrs 51 mins       ████████░░░░░░░░░░░░░░░░░   32.53 % 
Vim                      1 hr 55 mins        ████░░░░░░░░░░░░░░░░░░░░░   16.29 % 

💻 Operating System: 
Linux                    11 hrs 51 mins      █████████████████████████   100.00 % 
```


 Last Updated on 07/11/2023 00:10:16 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
