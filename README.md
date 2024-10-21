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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C858%20hrs%2044%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1644 commits        ██████░░░░░░░░░░░░░░░░░░░   25.27 % 
🌆 Daytime                2778 commits        ███████████░░░░░░░░░░░░░░   42.69 % 
🌃 Evening                1837 commits        ███████░░░░░░░░░░░░░░░░░░   28.23 % 
🌙 Night                  248 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.81 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   928 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.26 % 
Tuesday                  880 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.52 % 
Wednesday                862 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.25 % 
Thursday                 871 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.39 % 
Friday                   876 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.46 % 
Saturday                 1014 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.58 % 
Sunday                   1076 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.54 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       11 hrs 59 mins      ████████████░░░░░░░░░░░░░   49.66 % 
YAML                     8 hrs 50 mins       █████████░░░░░░░░░░░░░░░░   36.63 % 
Markdown                 1 hr 41 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   07.02 % 
Bash                     1 hr 1 min          █░░░░░░░░░░░░░░░░░░░░░░░░   04.24 % 
Other                    11 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   00.78 % 

🔥 Editors: 
Zsh                      11 hrs 59 mins      ████████████░░░░░░░░░░░░░   49.66 % 
VS Code                  11 hrs 6 mins       ████████████░░░░░░░░░░░░░   46.01 % 
Obsidian                 57 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.99 % 
Vim                      4 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.34 % 

💻 Operating System: 
Linux                    24 hrs 8 mins       █████████████████████████   100.00 % 
```


 Last Updated on 21/10/2024 00:49:35 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
