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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C431%20hrs%2029%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1537 commits        ██████░░░░░░░░░░░░░░░░░░░   22.84 % 
🌆 Daytime                3000 commits        ███████████░░░░░░░░░░░░░░   44.59 % 
🌃 Evening                1958 commits        ███████░░░░░░░░░░░░░░░░░░   29.10 % 
🌙 Night                  233 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.46 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   942 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.00 % 
Tuesday                  839 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.47 % 
Wednesday                890 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.23 % 
Thursday                 942 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.00 % 
Friday                   861 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.80 % 
Saturday                 1019 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.15 % 
Sunday                   1235 commits        █████░░░░░░░░░░░░░░░░░░░░   18.36 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
YAML                     1 hr 53 mins        ███████░░░░░░░░░░░░░░░░░░   28.33 % 
Markdown                 1 hr 48 mins        ███████░░░░░░░░░░░░░░░░░░   27.00 % 
Bash                     1 hr 5 mins         ████░░░░░░░░░░░░░░░░░░░░░   16.28 % 
Other                    56 mins             ████░░░░░░░░░░░░░░░░░░░░░   14.08 % 
INI                      20 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   05.14 % 

🔥 Editors: 
VS Code                  5 hrs 43 mins       █████████████████████░░░░   85.66 % 
Obsidian                 47 mins             ███░░░░░░░░░░░░░░░░░░░░░░   11.77 % 
Vim                      10 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.57 % 

💻 Operating System: 
Linux                    6 hrs 40 mins       █████████████████████████   100.00 % 
```


 Last Updated on 09/03/2024 00:08:50 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
