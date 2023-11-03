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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C304%20hrs%2034%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1486 commits        ██████░░░░░░░░░░░░░░░░░░░   22.54 % 
🌆 Daytime                2963 commits        ███████████░░░░░░░░░░░░░░   44.94 % 
🌃 Evening                1917 commits        ███████░░░░░░░░░░░░░░░░░░   29.08 % 
🌙 Night                  227 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.44 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   963 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.61 % 
Tuesday                  843 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.79 % 
Wednesday                842 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.77 % 
Thursday                 925 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.03 % 
Friday                   850 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.89 % 
Saturday                 983 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.91 % 
Sunday                   1187 commits        ████░░░░░░░░░░░░░░░░░░░░░   18.00 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
YAML                     4 hrs 19 mins       ██████████░░░░░░░░░░░░░░░   41.12 % 
Markdown                 2 hrs 58 mins       ███████░░░░░░░░░░░░░░░░░░   28.35 % 
Other                    58 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   09.32 % 
conf                     49 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   07.84 % 
Bash                     33 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   05.36 % 

🔥 Editors: 
VS Code                  5 hrs 54 mins       ██████████████░░░░░░░░░░░   56.11 % 
Obsidian                 2 hrs 31 mins       ██████░░░░░░░░░░░░░░░░░░░   24.05 % 
Vim                      1 hr 57 mins        █████░░░░░░░░░░░░░░░░░░░░   18.63 % 
Sublime Text             7 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   01.22 % 

💻 Operating System: 
Linux                    10 hrs 30 mins      █████████████████████████   100.00 % 
```


 Last Updated on 03/11/2023 00:09:45 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
