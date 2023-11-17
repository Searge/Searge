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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C320%20hrs%2051%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1502 commits        ██████░░░░░░░░░░░░░░░░░░░   22.56 % 
🌆 Daytime                2999 commits        ███████████░░░░░░░░░░░░░░   45.04 % 
🌃 Evening                1928 commits        ███████░░░░░░░░░░░░░░░░░░   28.96 % 
🌙 Night                  229 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.44 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   980 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.72 % 
Tuesday                  855 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.84 % 
Wednesday                842 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.65 % 
Thursday                 928 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.94 % 
Friday                   850 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.77 % 
Saturday                 983 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.76 % 
Sunday                   1220 commits        █████░░░░░░░░░░░░░░░░░░░░   18.32 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 2 hrs 22 mins       ████████████░░░░░░░░░░░░░   49.31 % 
YAML                     1 hr 1 min          █████░░░░░░░░░░░░░░░░░░░░   21.18 % 
VCL                      30 mins             ███░░░░░░░░░░░░░░░░░░░░░░   10.41 % 
Bash                     26 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   09.27 % 
Other                    21 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   07.46 % 

🔥 Editors: 
VS Code                  2 hrs 24 mins       █████████████░░░░░░░░░░░░   50.25 % 
Obsidian                 2 hrs 8 mins        ███████████░░░░░░░░░░░░░░   44.62 % 
Sublime Text             12 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.19 % 
Vim                      2 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.93 % 

💻 Operating System: 
Linux                    4 hrs 48 mins       █████████████████████████   100.00 % 
```


 Last Updated on 17/11/2023 00:10:29 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
