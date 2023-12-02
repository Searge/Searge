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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C343%20hrs%2052%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1507 commits        ██████░░░░░░░░░░░░░░░░░░░   22.56 % 
🌆 Daytime                3012 commits        ███████████░░░░░░░░░░░░░░   45.09 % 
🌃 Evening                1931 commits        ███████░░░░░░░░░░░░░░░░░░   28.91 % 
🌙 Night                  230 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.44 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   983 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.72 % 
Tuesday                  855 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.80 % 
Wednesday                842 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.60 % 
Thursday                 928 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.89 % 
Friday                   850 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.72 % 
Saturday                 985 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.75 % 
Sunday                   1237 commits        █████░░░░░░░░░░░░░░░░░░░░   18.52 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 4 hrs 41 mins       ███████████░░░░░░░░░░░░░░   44.97 % 
Other                    2 hrs 29 mins       ██████░░░░░░░░░░░░░░░░░░░   23.91 % 
INI                      1 hr 20 mins        ███░░░░░░░░░░░░░░░░░░░░░░   12.81 % 
YAML                     1 hr 5 mins         ███░░░░░░░░░░░░░░░░░░░░░░   10.41 % 
Bash                     26 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.29 % 

🔥 Editors: 
VS Code                  6 hrs 1 min         ██████████████░░░░░░░░░░░   57.61 % 
Obsidian                 4 hrs 25 mins       ███████████░░░░░░░░░░░░░░   42.33 % 
Vim                      0 secs              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.07 % 

💻 Operating System: 
Linux                    10 hrs 27 mins      █████████████████████████   100.00 % 
```


 Last Updated on 02/12/2023 00:10:07 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
