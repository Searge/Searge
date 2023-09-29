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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C239%20hrs%206%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1364 commits        ██████░░░░░░░░░░░░░░░░░░░   22.61 % 
🌆 Daytime                2719 commits        ███████████░░░░░░░░░░░░░░   45.06 % 
🌃 Evening                1730 commits        ███████░░░░░░░░░░░░░░░░░░   28.67 % 
🌙 Night                  221 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.66 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   853 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.14 % 
Tuesday                  779 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.91 % 
Wednesday                800 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.26 % 
Thursday                 855 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.17 % 
Friday                   816 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.52 % 
Saturday                 927 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.36 % 
Sunday                   1004 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.64 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
YAML                     2 hrs 10 mins       ████████░░░░░░░░░░░░░░░░░   33.22 % 
Markdown                 1 hr 18 mins        █████░░░░░░░░░░░░░░░░░░░░   19.90 % 
Docker                   1 hr 17 mins        █████░░░░░░░░░░░░░░░░░░░░   19.75 % 
Bash                     1 hr 12 mins        █████░░░░░░░░░░░░░░░░░░░░   18.54 % 
Go                       12 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.19 % 

🔥 Editors: 
VS Code                  5 hrs 21 mins       ████████████████████░░░░░   81.79 % 
Obsidian                 1 hr 6 mins         ████░░░░░░░░░░░░░░░░░░░░░   16.97 % 
Vim                      4 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   01.24 % 

💻 Operating System: 
Linux                    6 hrs 32 mins       █████████████████████████   100.00 % 
```


 Last Updated on 29/09/2023 00:09:27 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
