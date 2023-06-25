# Hi, I'm Searge <img src="images/vulcan.webp" style="display: inline-block; margin: 0; height: 2rem" alt="Vulcan salute" />

## An DevOps Engineer at [Smile Ukraine](https://smile-ukraine.com/en)

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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C097%20hrs%2043%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1210 commits        ██████░░░░░░░░░░░░░░░░░░░   22.16 % 
🌆 Daytime                2455 commits        ███████████░░░░░░░░░░░░░░   44.96 % 
🌃 Evening                1594 commits        ███████░░░░░░░░░░░░░░░░░░   29.19 % 
🌙 Night                  201 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.68 % 
```
📅 **I'm Most Productive on Saturday** 

```text
Monday                   782 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.32 % 
Tuesday                  729 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.35 % 
Wednesday                716 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.11 % 
Thursday                 781 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.30 % 
Friday                   785 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.38 % 
Saturday                 860 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.75 % 
Sunday                   807 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.78 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 6 hrs 40 mins       ██████████████░░░░░░░░░░░   57.33 % 
INI                      2 hrs 20 mins       █████░░░░░░░░░░░░░░░░░░░░   20.06 % 
Other                    55 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   07.92 % 
Bash                     36 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   05.26 % 
VCL                      26 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.79 % 

🔥 Editors: 
VS Code                  5 hrs 51 mins       █████████████░░░░░░░░░░░░   50.23 % 
Obsidian                 5 hrs 16 mins       ███████████░░░░░░░░░░░░░░   45.23 % 
Vim                      31 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.54 % 

💻 Operating System: 
Linux                    11 hrs 21 mins      ████████████████████████░   97.39 % 
Mac                      18 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.61 % 
```


 Last Updated on 25/06/2023 13:05:32 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
