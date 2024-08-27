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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C734%20hrs%2045%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1601 commits        ██████░░░░░░░░░░░░░░░░░░░   24.62 % 
🌆 Daytime                2818 commits        ███████████░░░░░░░░░░░░░░   43.33 % 
🌃 Evening                1841 commits        ███████░░░░░░░░░░░░░░░░░░   28.31 % 
🌙 Night                  244 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.75 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   971 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.93 % 
Tuesday                  910 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.99 % 
Wednesday                816 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.55 % 
Thursday                 862 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.25 % 
Friday                   857 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.18 % 
Saturday                 1011 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.54 % 
Sunday                   1077 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.56 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       2 hrs 2 mins        █████████████░░░░░░░░░░░░   51.61 % 
Markdown                 1 hr 5 mins         ███████░░░░░░░░░░░░░░░░░░   27.60 % 
YAML                     26 mins             ███░░░░░░░░░░░░░░░░░░░░░░   11.29 % 
INI                      8 mins              █░░░░░░░░░░░░░░░░░░░░░░░░   03.57 % 
Docker                   6 mins              █░░░░░░░░░░░░░░░░░░░░░░░░   02.65 % 

🔥 Editors: 
Zsh                      2 hrs               █████████████░░░░░░░░░░░░   50.69 % 
VS Code                  1 hr 54 mins        ████████████░░░░░░░░░░░░░   48.13 % 
Vim                      2 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   01.18 % 

💻 Operating System: 
Linux                    3 hrs 57 mins       █████████████████████████   100.00 % 
```


 Last Updated on 27/08/2024 00:45:27 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
