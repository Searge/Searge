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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C728%20hrs%202%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1634 commits        ██████░░░░░░░░░░░░░░░░░░░   24.68 % 
🌆 Daytime                2866 commits        ███████████░░░░░░░░░░░░░░   43.29 % 
🌃 Evening                1876 commits        ███████░░░░░░░░░░░░░░░░░░   28.34 % 
🌙 Night                  244 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.69 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   997 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.06 % 
Tuesday                  949 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.34 % 
Wednesday                828 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.51 % 
Thursday                 877 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.25 % 
Friday                   860 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.99 % 
Saturday                 1032 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.59 % 
Sunday                   1077 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.27 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       6 hrs 15 mins       ██████████████░░░░░░░░░░░   56.36 % 
YAML                     2 hrs 35 mins       ██████░░░░░░░░░░░░░░░░░░░   23.39 % 
Markdown                 58 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   08.85 % 
Bash                     29 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.43 % 
Smarty                   25 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.86 % 

🔥 Editors: 
Zsh                      6 hrs 15 mins       ██████████████░░░░░░░░░░░   56.36 % 
VS Code                  3 hrs 52 mins       █████████░░░░░░░░░░░░░░░░   34.92 % 
Obsidian                 57 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   08.62 % 
Vim                      0 secs              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.10 % 

💻 Operating System: 
Linux                    11 hrs 5 mins       █████████████████████████   100.00 % 
```


 Last Updated on 20/08/2024 00:44:43 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
