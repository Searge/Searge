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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C448%20hrs%2031%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1405 commits        ██████░░░░░░░░░░░░░░░░░░░   23.71 % 
🌆 Daytime                2635 commits        ███████████░░░░░░░░░░░░░░   44.46 % 
🌃 Evening                1654 commits        ███████░░░░░░░░░░░░░░░░░░   27.91 % 
🌙 Night                  233 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.93 % 
```
📅 **I'm Most Productive on Saturday** 

```text
Monday                   845 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.26 % 
Tuesday                  792 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.36 % 
Wednesday                805 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.58 % 
Thursday                 825 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.92 % 
Friday                   827 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.95 % 
Saturday                 917 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.47 % 
Sunday                   916 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.45 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 50 mins             ███████████████████████░░   92.17 % 
Bash                     2 mins              █░░░░░░░░░░░░░░░░░░░░░░░░   05.21 % 
INI                      0 secs              ░░░░░░░░░░░░░░░░░░░░░░░░░   01.18 % 
YAML                     0 secs              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.83 % 
fish                     0 secs              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.61 % 

🔥 Editors: 
Obsidian                 30 mins             ██████████████░░░░░░░░░░░   55.89 % 
VS Code                  23 mins             ███████████░░░░░░░░░░░░░░   43.50 % 
Vim                      0 secs              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.61 % 

💻 Operating System: 
Linux                    54 mins             █████████████████████████   100.00 % 
```


 Last Updated on 04/04/2024 00:37:02 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
