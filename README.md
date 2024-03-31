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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C448%20hrs%2021%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1543 commits        ██████░░░░░░░░░░░░░░░░░░░   22.87 % 
🌆 Daytime                3007 commits        ███████████░░░░░░░░░░░░░░   44.57 % 
🌃 Evening                1964 commits        ███████░░░░░░░░░░░░░░░░░░   29.11 % 
🌙 Night                  233 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.45 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   946 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.02 % 
Tuesday                  845 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.52 % 
Wednesday                890 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.19 % 
Thursday                 943 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.98 % 
Friday                   863 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.79 % 
Saturday                 1025 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.19 % 
Sunday                   1235 commits        █████░░░░░░░░░░░░░░░░░░░░   18.30 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 48 mins             █████████████░░░░░░░░░░░░   53.08 % 
Other                    21 mins             ██████░░░░░░░░░░░░░░░░░░░   23.66 % 
desktop                  16 mins             █████░░░░░░░░░░░░░░░░░░░░   18.13 % 
Lua                      2 mins              █░░░░░░░░░░░░░░░░░░░░░░░░   02.36 % 
INI                      1 min               ░░░░░░░░░░░░░░░░░░░░░░░░░   01.51 % 

🔥 Editors: 
Obsidian                 28 mins             ████████░░░░░░░░░░░░░░░░░   31.75 % 
Vim                      26 mins             ███████░░░░░░░░░░░░░░░░░░   29.69 % 
VS Code                  21 mins             ██████░░░░░░░░░░░░░░░░░░░   23.63 % 
Sublime Text             13 mins             ████░░░░░░░░░░░░░░░░░░░░░   14.94 % 

💻 Operating System: 
Linux                    1 hr 30 mins        █████████████████████████   100.00 % 
```


 Last Updated on 31/03/2024 00:36:17 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
