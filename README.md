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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C650%20hrs%2056%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1599 commits        ██████░░░░░░░░░░░░░░░░░░░   24.66 % 
🌆 Daytime                2784 commits        ███████████░░░░░░░░░░░░░░   42.94 % 
🌃 Evening                1856 commits        ███████░░░░░░░░░░░░░░░░░░   28.62 % 
🌙 Night                  245 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.78 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   955 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.73 % 
Tuesday                  897 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.83 % 
Wednesday                800 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.34 % 
Thursday                 843 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.00 % 
Friday                   834 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.86 % 
Saturday                 1057 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.30 % 
Sunday                   1098 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.93 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       9 hrs 35 mins       █████████████████░░░░░░░░   69.75 % 
YAML                     2 hrs 29 mins       █████░░░░░░░░░░░░░░░░░░░░   18.14 % 
Markdown                 1 hr 21 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   09.92 % 
Other                    14 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.78 % 
desktop                  1 min               ░░░░░░░░░░░░░░░░░░░░░░░░░   00.21 % 

🔥 Editors: 
Zsh                      9 hrs 35 mins       █████████████████░░░░░░░░   69.75 % 
VS Code                  3 hrs 1 min         █████░░░░░░░░░░░░░░░░░░░░   21.98 % 
Obsidian                 1 hr 1 min          ██░░░░░░░░░░░░░░░░░░░░░░░   07.41 % 
Vim                      7 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.86 % 

💻 Operating System: 
Linux                    13 hrs 44 mins      █████████████████████████   100.00 % 
```


 Last Updated on 11/07/2024 00:45:00 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
