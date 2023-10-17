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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C282%20hrs%2032%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1438 commits        ██████░░░░░░░░░░░░░░░░░░░   22.42 % 
🌆 Daytime                2889 commits        ███████████░░░░░░░░░░░░░░   45.05 % 
🌃 Evening                1859 commits        ███████░░░░░░░░░░░░░░░░░░   28.99 % 
🌙 Night                  227 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.54 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   937 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.61 % 
Tuesday                  821 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.80 % 
Wednesday                828 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.91 % 
Thursday                 903 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.08 % 
Friday                   826 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.88 % 
Saturday                 965 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.05 % 
Sunday                   1133 commits        ████░░░░░░░░░░░░░░░░░░░░░   17.67 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
YAML                     4 hrs 7 mins        ██████░░░░░░░░░░░░░░░░░░░   22.65 % 
Terraform                2 hrs 22 mins       ███░░░░░░░░░░░░░░░░░░░░░░   13.03 % 
Bash                     2 hrs 5 mins        ███░░░░░░░░░░░░░░░░░░░░░░   11.52 % 
GDScript                 1 hr 53 mins        ███░░░░░░░░░░░░░░░░░░░░░░   10.38 % 
Markdown                 1 hr 41 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   09.33 % 

🔥 Editors: 
VS Code                  16 hrs 32 mins      ███████████████████████░░   90.85 % 
Obsidian                 1 hr 9 mins         ██░░░░░░░░░░░░░░░░░░░░░░░   06.38 % 
Vim                      30 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.77 % 

💻 Operating System: 
Linux                    18 hrs 12 mins      █████████████████████████   100.00 % 
```


 Last Updated on 17/10/2023 00:10:00 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
