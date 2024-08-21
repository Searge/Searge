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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C731%20hrs%2057%20mins-blue)

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
sh                       6 hrs               ██████████████░░░░░░░░░░░   54.98 % 
YAML                     2 hrs 48 mins       ██████░░░░░░░░░░░░░░░░░░░   25.69 % 
Bash                     29 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.53 % 
Markdown                 28 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.42 % 
Smarty                   25 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.92 % 

🔥 Editors: 
Zsh                      5 hrs 57 mins       ██████████████░░░░░░░░░░░   54.64 % 
VS Code                  4 hrs 30 mins       ██████████░░░░░░░░░░░░░░░   41.25 % 
Obsidian                 23 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.58 % 
Vim                      3 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.53 % 

💻 Operating System: 
Linux                    10 hrs 55 mins      █████████████████████████   100.00 % 
```


 Last Updated on 21/08/2024 00:44:32 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
