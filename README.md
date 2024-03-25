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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C447%20hrs%204%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1543 commits        ██████░░░░░░░░░░░░░░░░░░░   22.85 % 
🌆 Daytime                3010 commits        ███████████░░░░░░░░░░░░░░   44.58 % 
🌃 Evening                1966 commits        ███████░░░░░░░░░░░░░░░░░░   29.12 % 
🌙 Night                  233 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.45 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   950 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.07 % 
Tuesday                  849 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.57 % 
Wednesday                890 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.18 % 
Thursday                 944 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.98 % 
Friday                   861 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.75 % 
Saturday                 1023 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.15 % 
Sunday                   1235 commits        █████░░░░░░░░░░░░░░░░░░░░   18.29 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
YAML                     1 hr 47 mins        ████████░░░░░░░░░░░░░░░░░   30.94 % 
Markdown                 1 hr 13 mins        █████░░░░░░░░░░░░░░░░░░░░   21.16 % 
fish                     51 mins             ████░░░░░░░░░░░░░░░░░░░░░   14.70 % 
TOML                     47 mins             ███░░░░░░░░░░░░░░░░░░░░░░   13.60 % 
Java                     28 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   08.12 % 

🔥 Editors: 
VS Code                  3 hrs 47 mins       ████████████████░░░░░░░░░   65.41 % 
Obsidian                 1 hr 8 mins         █████░░░░░░░░░░░░░░░░░░░░   19.68 % 
Vim                      38 mins             ███░░░░░░░░░░░░░░░░░░░░░░   11.03 % 
Sublime Text             13 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.88 % 

💻 Operating System: 
Linux                    5 hrs 48 mins       █████████████████████████   100.00 % 
```


 Last Updated on 25/03/2024 00:09:48 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
