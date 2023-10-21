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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C288%20hrs%2032%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1439 commits        ██████░░░░░░░░░░░░░░░░░░░   22.60 % 
🌆 Daytime                2865 commits        ███████████░░░░░░░░░░░░░░   44.99 % 
🌃 Evening                1837 commits        ███████░░░░░░░░░░░░░░░░░░   28.85 % 
🌙 Night                  227 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.56 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   932 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.64 % 
Tuesday                  827 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.99 % 
Wednesday                821 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.89 % 
Thursday                 894 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.04 % 
Friday                   832 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.07 % 
Saturday                 956 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.01 % 
Sunday                   1106 commits        ████░░░░░░░░░░░░░░░░░░░░░   17.37 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Terraform                2 hrs 50 mins       ██████░░░░░░░░░░░░░░░░░░░   25.22 % 
YAML                     2 hrs 12 mins       █████░░░░░░░░░░░░░░░░░░░░   19.68 % 
Markdown                 1 hr 41 mins        ████░░░░░░░░░░░░░░░░░░░░░   15.05 % 
GDScript                 1 hr 19 mins        ███░░░░░░░░░░░░░░░░░░░░░░   11.77 % 
Bash                     56 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   08.39 % 

🔥 Editors: 
VS Code                  9 hrs 23 mins       █████████████████████░░░░   83.48 % 
Obsidian                 1 hr 4 mins         ██░░░░░░░░░░░░░░░░░░░░░░░   09.63 % 
Vim                      37 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   05.61 % 
Sublime Text             8 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   01.28 % 

💻 Operating System: 
Linux                    11 hrs 15 mins      █████████████████████████   100.00 % 
```


 Last Updated on 21/10/2023 00:09:24 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
