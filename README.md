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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C415%20hrs-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1544 commits        ██████░░░░░░░░░░░░░░░░░░░   22.76 % 
🌆 Daytime                3039 commits        ███████████░░░░░░░░░░░░░░   44.80 % 
🌃 Evening                1968 commits        ███████░░░░░░░░░░░░░░░░░░   29.01 % 
🌙 Night                  233 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.43 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   1005 commits        ████░░░░░░░░░░░░░░░░░░░░░   14.81 % 
Tuesday                  903 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.31 % 
Wednesday                880 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.97 % 
Thursday                 945 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.93 % 
Friday                   854 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.59 % 
Saturday                 998 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.71 % 
Sunday                   1199 commits        ████░░░░░░░░░░░░░░░░░░░░░   17.67 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 1 hr 30 mins        ████████████░░░░░░░░░░░░░   47.31 % 
gitrebase                42 mins             ██████░░░░░░░░░░░░░░░░░░░   22.09 % 
Git                      14 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   07.75 % 
TOML                     13 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   07.28 % 
Other                    7 mins              █░░░░░░░░░░░░░░░░░░░░░░░░   04.10 % 

🔥 Editors: 
Obsidian                 1 hr 29 mins        ████████████░░░░░░░░░░░░░   46.79 % 
Vim                      1 hr 5 mins         █████████░░░░░░░░░░░░░░░░   34.31 % 
VS Code                  35 mins             █████░░░░░░░░░░░░░░░░░░░░   18.90 % 

💻 Operating System: 
Linux                    3 hrs 10 mins       █████████████████████████   100.00 % 
```


 Last Updated on 09/02/2024 00:09:42 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
