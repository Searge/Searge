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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C900%20hrs%2053%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1924 commits        ██████░░░░░░░░░░░░░░░░░░░   25.85 % 
🌆 Daytime                2933 commits        ██████████░░░░░░░░░░░░░░░   39.41 % 
🌃 Evening                2288 commits        ████████░░░░░░░░░░░░░░░░░   30.74 % 
🌙 Night                  298 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   04.00 % 
```
📅 **I'm Most Productive on Saturday** 

```text
Monday                   1012 commits        ███░░░░░░░░░░░░░░░░░░░░░░   13.60 % 
Tuesday                  920 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.36 % 
Wednesday                935 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.56 % 
Thursday                 923 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.40 % 
Friday                   900 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.09 % 
Saturday                 1407 commits        █████░░░░░░░░░░░░░░░░░░░░   18.90 % 
Sunday                   1346 commits        █████░░░░░░░░░░░░░░░░░░░░   18.08 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       6 hrs 52 mins       ██████████████░░░░░░░░░░░   55.44 % 
YAML                     3 hrs 31 mins       ███████░░░░░░░░░░░░░░░░░░   28.48 % 
Markdown                 26 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.62 % 
Other                    25 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.46 % 
Jinja2                   22 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.01 % 

🔥 Editors: 
Zsh                      6 hrs 52 mins       ██████████████░░░░░░░░░░░   55.44 % 
Cursor                   3 hrs 8 mins        ██████░░░░░░░░░░░░░░░░░░░   25.40 % 
VS Code                  2 hrs 4 mins        ████░░░░░░░░░░░░░░░░░░░░░   16.79 % 
Obsidian                 17 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.38 % 

💻 Operating System: 
Linux                    12 hrs 23 mins      █████████████████████████   100.00 % 
```


 Last Updated on 04/11/2024 17:12:31 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
