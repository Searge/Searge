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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C347%20hrs%2047%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1504 commits        ██████░░░░░░░░░░░░░░░░░░░   22.56 % 
🌆 Daytime                3005 commits        ███████████░░░░░░░░░░░░░░   45.07 % 
🌃 Evening                1930 commits        ███████░░░░░░░░░░░░░░░░░░   28.94 % 
🌙 Night                  229 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.43 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   984 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.76 % 
Tuesday                  859 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.88 % 
Wednesday                842 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.63 % 
Thursday                 929 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.93 % 
Friday                   850 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.75 % 
Saturday                 984 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.76 % 
Sunday                   1220 commits        █████░░░░░░░░░░░░░░░░░░░░   18.30 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 2 hrs 58 mins       ███████████████████░░░░░░   75.70 % 
Other                    18 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   07.81 % 
SSH Config               12 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   05.42 % 
YAML                     9 mins              █░░░░░░░░░░░░░░░░░░░░░░░░   04.25 % 
Bash                     9 mins              █░░░░░░░░░░░░░░░░░░░░░░░░   03.98 % 

🔥 Editors: 
Obsidian                 2 hrs 12 mins       ██████████████░░░░░░░░░░░   56.28 % 
VS Code                  1 hr 28 mins        █████████░░░░░░░░░░░░░░░░   37.52 % 
Sublime Text             7 mins              █░░░░░░░░░░░░░░░░░░░░░░░░   03.38 % 
Vim                      6 mins              █░░░░░░░░░░░░░░░░░░░░░░░░   02.82 % 

💻 Operating System: 
Linux                    3 hrs 55 mins       █████████████████████████   100.00 % 
```


 Last Updated on 09/12/2023 00:09:43 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
