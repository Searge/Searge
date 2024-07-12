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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C652%20hrs%2040%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1564 commits        ██████░░░░░░░░░░░░░░░░░░░   24.53 % 
🌆 Daytime                2763 commits        ███████████░░░░░░░░░░░░░░   43.33 % 
🌃 Evening                1808 commits        ███████░░░░░░░░░░░░░░░░░░   28.36 % 
🌙 Night                  241 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.78 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   944 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.81 % 
Tuesday                  886 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.90 % 
Wednesday                792 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.42 % 
Thursday                 847 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.28 % 
Friday                   831 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.03 % 
Saturday                 1005 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.76 % 
Sunday                   1071 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.80 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       8 hrs 54 mins       █████████████████████░░░░   84.54 % 
YAML                     48 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   07.64 % 
Markdown                 31 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   05.02 % 
Other                    15 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.41 % 
desktop                  1 min               ░░░░░░░░░░░░░░░░░░░░░░░░░   00.27 % 

🔥 Editors: 
Zsh                      8 hrs 54 mins       █████████████████████░░░░   84.54 % 
VS Code                  1 hr 1 min          ██░░░░░░░░░░░░░░░░░░░░░░░   09.67 % 
Obsidian                 31 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.99 % 
Vim                      5 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.80 % 

💻 Operating System: 
Linux                    10 hrs 32 mins      █████████████████████████   100.00 % 
```


 Last Updated on 12/07/2024 00:45:01 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
