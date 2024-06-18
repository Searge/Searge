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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C594%20hrs%2035%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1527 commits        ██████░░░░░░░░░░░░░░░░░░░   24.21 % 
🌆 Daytime                2714 commits        ███████████░░░░░░░░░░░░░░   43.03 % 
🌃 Evening                1823 commits        ███████░░░░░░░░░░░░░░░░░░   28.90 % 
🌙 Night                  243 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.85 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   914 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.49 % 
Tuesday                  852 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.51 % 
Wednesday                795 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.61 % 
Thursday                 830 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.16 % 
Friday                   827 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.11 % 
Saturday                 1037 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.44 % 
Sunday                   1052 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.68 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       8 hrs 42 mins       ██████████████████░░░░░░░   73.52 % 
YAML                     1 hr 26 mins        ███░░░░░░░░░░░░░░░░░░░░░░   12.11 % 
Other                    38 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   05.42 % 
XML                      35 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.99 % 
XSLT                     17 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.51 % 

🔥 Editors: 
Zsh                      8 hrs 42 mins       ██████████████████░░░░░░░   73.52 % 
VS Code                  3 hrs 2 mins        ██████░░░░░░░░░░░░░░░░░░░   25.66 % 
Vim                      4 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.58 % 
Obsidian                 1 min               ░░░░░░░░░░░░░░░░░░░░░░░░░   00.24 % 

💻 Operating System: 
Linux                    11 hrs 50 mins      █████████████████████████   100.00 % 
```


 Last Updated on 18/06/2024 00:40:49 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
