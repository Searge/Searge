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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C512%20hrs%201%20min-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1508 commits        ██████░░░░░░░░░░░░░░░░░░░   24.16 % 
🌆 Daytime                2716 commits        ███████████░░░░░░░░░░░░░░   43.52 % 
🌃 Evening                1768 commits        ███████░░░░░░░░░░░░░░░░░░   28.33 % 
🌙 Night                  249 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.99 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   889 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.24 % 
Tuesday                  825 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.22 % 
Wednesday                836 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.40 % 
Thursday                 841 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.48 % 
Friday                   853 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.67 % 
Saturday                 985 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.78 % 
Sunday                   1012 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.22 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
YAML                     10 hrs 34 mins      ███████████░░░░░░░░░░░░░░   42.10 % 
sh                       9 hrs 16 mins       █████████░░░░░░░░░░░░░░░░   36.96 % 
Markdown                 1 hr 41 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   06.76 % 
Go                       1 hr 31 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   06.10 % 
Bash                     36 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.43 % 

🔥 Editors: 
VS Code                  14 hrs 2 mins       ██████████████░░░░░░░░░░░   55.90 % 
Zsh                      9 hrs 16 mins       █████████░░░░░░░░░░░░░░░░   36.96 % 
Obsidian                 1 hr 24 mins        █░░░░░░░░░░░░░░░░░░░░░░░░   05.60 % 
Vim                      20 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.37 % 
Sublime Text             2 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.17 % 

💻 Operating System: 
Linux                    25 hrs 6 mins       █████████████████████████   100.00 % 
```


 Last Updated on 20/05/2024 00:37:42 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
