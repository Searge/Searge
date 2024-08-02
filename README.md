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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C688%20hrs%2033%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1576 commits        ██████░░░░░░░░░░░░░░░░░░░   24.40 % 
🌆 Daytime                2809 commits        ███████████░░░░░░░░░░░░░░   43.48 % 
🌃 Evening                1834 commits        ███████░░░░░░░░░░░░░░░░░░   28.39 % 
🌙 Night                  241 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.73 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   971 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.03 % 
Tuesday                  906 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.02 % 
Wednesday                800 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.38 % 
Thursday                 858 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.28 % 
Friday                   846 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.10 % 
Saturday                 1005 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.56 % 
Sunday                   1074 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.63 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       3 hrs 59 mins       ██████████░░░░░░░░░░░░░░░   41.32 % 
YAML                     3 hrs 56 mins       ██████████░░░░░░░░░░░░░░░   40.72 % 
Markdown                 56 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   09.83 % 
Smarty                   30 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   05.35 % 
systemd                  8 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   01.39 % 

🔥 Editors: 
VS Code                  4 hrs 37 mins       ████████████░░░░░░░░░░░░░   47.89 % 
Zsh                      3 hrs 59 mins       ██████████░░░░░░░░░░░░░░░   41.32 % 
Obsidian                 56 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   09.77 % 
Vim                      5 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   01.02 % 

💻 Operating System: 
Linux                    9 hrs 39 mins       █████████████████████████   100.00 % 
```


 Last Updated on 02/08/2024 00:45:52 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
