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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C873%20hrs%2032%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1649 commits        ██████░░░░░░░░░░░░░░░░░░░   25.28 % 
🌆 Daytime                2786 commits        ███████████░░░░░░░░░░░░░░   42.70 % 
🌃 Evening                1841 commits        ███████░░░░░░░░░░░░░░░░░░   28.22 % 
🌙 Night                  248 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.80 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   934 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.32 % 
Tuesday                  885 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.57 % 
Wednesday                865 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.26 % 
Thursday                 872 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.37 % 
Friday                   878 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.46 % 
Saturday                 1014 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.54 % 
Sunday                   1076 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.49 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       14 hrs 54 mins      ███████████████░░░░░░░░░░   59.61 % 
YAML                     7 hrs 51 mins       ████████░░░░░░░░░░░░░░░░░   31.44 % 
Markdown                 1 hr 25 mins        █░░░░░░░░░░░░░░░░░░░░░░░░   05.70 % 
Other                    19 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.32 % 
Elixir                   10 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   00.73 % 

🔥 Editors: 
Zsh                      14 hrs 54 mins      ███████████████░░░░░░░░░░   59.61 % 
VS Code                  8 hrs 45 mins       █████████░░░░░░░░░░░░░░░░   35.04 % 
Obsidian                 1 hr 5 mins         █░░░░░░░░░░░░░░░░░░░░░░░░   04.37 % 
Vim                      9 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.60 % 
Cursor                   5 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.37 % 

💻 Operating System: 
Linux                    25 hrs              █████████████████████████   100.00 % 
```


 Last Updated on 26/10/2024 00:52:09 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
