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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C813%20hrs%201%20min-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1661 commits        ██████░░░░░░░░░░░░░░░░░░░   25.11 % 
🌆 Daytime                2851 commits        ███████████░░░░░░░░░░░░░░   43.10 % 
🌃 Evening                1855 commits        ███████░░░░░░░░░░░░░░░░░░   28.04 % 
🌙 Night                  248 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.75 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   973 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.71 % 
Tuesday                  939 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.20 % 
Wednesday                845 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.77 % 
Thursday                 886 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.39 % 
Friday                   878 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.27 % 
Saturday                 1023 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.46 % 
Sunday                   1071 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.19 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       9 hrs 49 mins       ████████████░░░░░░░░░░░░░   46.03 % 
YAML                     7 hrs 34 mins       █████████░░░░░░░░░░░░░░░░   35.43 % 
Markdown                 2 hrs 46 mins       ███░░░░░░░░░░░░░░░░░░░░░░   13.02 % 
Docker                   26 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.07 % 
Bash                     17 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.34 % 

🔥 Editors: 
VS Code                  10 hrs 4 mins       ████████████░░░░░░░░░░░░░   47.16 % 
Zsh                      9 hrs 49 mins       ████████████░░░░░░░░░░░░░   46.03 % 
Obsidian                 1 hr 16 mins        █░░░░░░░░░░░░░░░░░░░░░░░░   05.96 % 
Vim                      10 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   00.85 % 

💻 Operating System: 
Linux                    21 hrs 21 mins      █████████████████████████   100.00 % 
```


 Last Updated on 06/10/2024 00:51:18 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
