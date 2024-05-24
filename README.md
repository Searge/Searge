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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C521%20hrs%2056%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1490 commits        ██████░░░░░░░░░░░░░░░░░░░   24.16 % 
🌆 Daytime                2679 commits        ███████████░░░░░░░░░░░░░░   43.45 % 
🌃 Evening                1757 commits        ███████░░░░░░░░░░░░░░░░░░   28.49 % 
🌙 Night                  240 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.89 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   892 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.47 % 
Tuesday                  834 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.53 % 
Wednesday                800 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.97 % 
Thursday                 826 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.40 % 
Friday                   829 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.44 % 
Saturday                 973 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.78 % 
Sunday                   1012 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.41 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
YAML                     10 hrs 9 mins       ███████████░░░░░░░░░░░░░░   42.74 % 
sh                       10 hrs              ███████████░░░░░░░░░░░░░░   42.15 % 
Markdown                 59 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.17 % 
Go                       56 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.96 % 
Nix                      29 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.08 % 

🔥 Editors: 
VS Code                  13 hrs 1 min        ██████████████░░░░░░░░░░░   54.84 % 
Zsh                      10 hrs              ███████████░░░░░░░░░░░░░░   42.15 % 
Obsidian                 42 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.96 % 
Vim                      0 secs              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.05 % 

💻 Operating System: 
Linux                    23 hrs 45 mins      █████████████████████████   100.00 % 
```


 Last Updated on 24/05/2024 00:38:45 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
