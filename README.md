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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C454%20hrs%2011%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1476 commits        ██████░░░░░░░░░░░░░░░░░░░   24.05 % 
🌆 Daytime                2670 commits        ███████████░░░░░░░░░░░░░░   43.50 % 
🌃 Evening                1747 commits        ███████░░░░░░░░░░░░░░░░░░   28.46 % 
🌙 Night                  245 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.99 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   873 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.22 % 
Tuesday                  808 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.16 % 
Wednesday                813 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.25 % 
Thursday                 828 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.49 % 
Friday                   837 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.64 % 
Saturday                 978 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.93 % 
Sunday                   1001 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.31 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 1 hr 44 mins        ██████████████░░░░░░░░░░░   55.33 % 
Other                    35 mins             █████░░░░░░░░░░░░░░░░░░░░   18.69 % 
gitrebase                21 mins             ███░░░░░░░░░░░░░░░░░░░░░░   11.37 % 
XML                      11 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   05.92 % 
Java Properties          9 mins              █░░░░░░░░░░░░░░░░░░░░░░░░   05.22 % 

🔥 Editors: 
Obsidian                 1 hr 32 mins        ████████████░░░░░░░░░░░░░   48.87 % 
VS Code                  1 hr 15 mins        ██████████░░░░░░░░░░░░░░░   39.54 % 
Vim                      21 mins             ███░░░░░░░░░░░░░░░░░░░░░░   11.59 % 

💻 Operating System: 
Linux                    3 hrs 9 mins        █████████████████████████   100.00 % 
```


 Last Updated on 18/04/2024 00:40:01 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
