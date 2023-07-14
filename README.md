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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C143%20hrs%2031%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1223 commits        ██████░░░░░░░░░░░░░░░░░░░   22.30 % 
🌆 Daytime                2465 commits        ███████████░░░░░░░░░░░░░░   44.95 % 
🌃 Evening                1586 commits        ███████░░░░░░░░░░░░░░░░░░   28.92 % 
🌙 Night                  210 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.83 % 
```
📅 **I'm Most Productive on Saturday** 

```text
Monday                   787 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.35 % 
Tuesday                  731 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.33 % 
Wednesday                718 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.09 % 
Thursday                 781 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.24 % 
Friday                   785 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.31 % 
Saturday                 849 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.48 % 
Sunday                   833 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.19 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
YAML                     5 hrs 49 mins       █████████░░░░░░░░░░░░░░░░   35.61 % 
Markdown                 4 hrs 35 mins       ███████░░░░░░░░░░░░░░░░░░   28.02 % 
Bash                     1 hr 38 mins        ███░░░░░░░░░░░░░░░░░░░░░░   10.06 % 
Terraform                1 hr 3 mins         ██░░░░░░░░░░░░░░░░░░░░░░░   06.44 % 
Other                    55 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   05.70 % 

🔥 Editors: 
VS Code                  12 hrs 35 mins      ███████████████████░░░░░░   77.01 % 
Obsidian                 3 hrs 45 mins       ██████░░░░░░░░░░░░░░░░░░░   22.99 % 

💻 Operating System: 
Linux                    16 hrs 21 mins      █████████████████████████   100.00 % 
```


 Last Updated on 14/07/2023 00:10:48 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
