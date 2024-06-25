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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C607%20hrs%2030%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1541 commits        ██████░░░░░░░░░░░░░░░░░░░   24.31 % 
🌆 Daytime                2727 commits        ███████████░░░░░░░░░░░░░░   43.01 % 
🌃 Evening                1829 commits        ███████░░░░░░░░░░░░░░░░░░   28.85 % 
🌙 Night                  243 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.83 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   922 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.54 % 
Tuesday                  866 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.66 % 
Wednesday                797 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.57 % 
Thursday                 831 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.11 % 
Friday                   827 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.04 % 
Saturday                 1045 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.48 % 
Sunday                   1052 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.59 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       11 hrs 42 mins      ██████████████████░░░░░░░   72.76 % 
YAML                     2 hrs 53 mins       ████░░░░░░░░░░░░░░░░░░░░░   17.92 % 
JSON                     32 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.39 % 
Other                    20 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.15 % 
Docker                   16 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.69 % 

🔥 Editors: 
Zsh                      11 hrs 42 mins      ██████████████████░░░░░░░   72.76 % 
VS Code                  4 hrs 16 mins       ███████░░░░░░░░░░░░░░░░░░   26.51 % 
Vim                      6 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.72 % 

💻 Operating System: 
Linux                    16 hrs 6 mins       █████████████████████████   100.00 % 
```


 Last Updated on 25/06/2024 00:42:34 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
