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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C657%20hrs%2027%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1564 commits        ██████░░░░░░░░░░░░░░░░░░░   24.53 % 
🌆 Daytime                2763 commits        ███████████░░░░░░░░░░░░░░   43.33 % 
🌃 Evening                1808 commits        ███████░░░░░░░░░░░░░░░░░░   28.36 % 
🌙 Night                  241 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.78 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   944 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.81 % 
Tuesday                  886 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.90 % 
Wednesday                792 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.42 % 
Thursday                 847 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.28 % 
Friday                   831 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.03 % 
Saturday                 1005 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.76 % 
Sunday                   1071 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.80 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       10 hrs 14 mins      █████████████████████░░░░   82.63 % 
YAML                     1 hr 17 mins        ███░░░░░░░░░░░░░░░░░░░░░░   10.38 % 
Markdown                 26 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.56 % 
Other                    15 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.05 % 
Lua                      3 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.50 % 

🔥 Editors: 
Zsh                      10 hrs 14 mins      █████████████████████░░░░   82.63 % 
VS Code                  1 hr 25 mins        ███░░░░░░░░░░░░░░░░░░░░░░   11.54 % 
Obsidian                 26 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.53 % 
Vim                      17 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.29 % 

💻 Operating System: 
Linux                    12 hrs 23 mins      █████████████████████████   100.00 % 
```


 Last Updated on 14/07/2024 00:42:14 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
