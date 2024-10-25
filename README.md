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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C869%20hrs%2033%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1645 commits        ██████░░░░░░░░░░░░░░░░░░░   25.26 % 
🌆 Daytime                2781 commits        ███████████░░░░░░░░░░░░░░   42.70 % 
🌃 Evening                1839 commits        ███████░░░░░░░░░░░░░░░░░░   28.24 % 
🌙 Night                  248 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.81 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   930 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.28 % 
Tuesday                  881 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.53 % 
Wednesday                865 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.28 % 
Thursday                 871 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.37 % 
Friday                   876 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.45 % 
Saturday                 1014 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.57 % 
Sunday                   1076 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.52 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       13 hrs 55 mins      █████████████████░░░░░░░░   66.73 % 
YAML                     4 hrs 38 mins       ██████░░░░░░░░░░░░░░░░░░░   22.23 % 
Markdown                 1 hr 22 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   06.59 % 
Bash                     23 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.84 % 
Elixir                   10 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   00.87 % 

🔥 Editors: 
Zsh                      13 hrs 55 mins      █████████████████░░░░░░░░   66.73 % 
VS Code                  5 hrs 36 mins       ███████░░░░░░░░░░░░░░░░░░   26.84 % 
Obsidian                 1 hr 6 mins         █░░░░░░░░░░░░░░░░░░░░░░░░   05.28 % 
Vim                      8 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.70 % 
Cursor                   5 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.45 % 

💻 Operating System: 
Linux                    20 hrs 52 mins      █████████████████████████   100.00 % 
```


 Last Updated on 25/10/2024 00:51:42 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
