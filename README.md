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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C883%20hrs%2045%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1653 commits        ██████░░░░░░░░░░░░░░░░░░░   25.24 % 
🌆 Daytime                2792 commits        ███████████░░░░░░░░░░░░░░   42.63 % 
🌃 Evening                1856 commits        ███████░░░░░░░░░░░░░░░░░░   28.34 % 
🌙 Night                  248 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.79 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   940 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.35 % 
Tuesday                  890 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.59 % 
Wednesday                865 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.21 % 
Thursday                 873 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.33 % 
Friday                   878 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.41 % 
Saturday                 1027 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.68 % 
Sunday                   1076 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.43 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       12 hrs 43 mins      ████████████░░░░░░░░░░░░░   48.93 % 
YAML                     9 hrs 4 mins        █████████░░░░░░░░░░░░░░░░   34.85 % 
Other                    1 hr 28 mins        █░░░░░░░░░░░░░░░░░░░░░░░░   05.68 % 
Markdown                 1 hr 22 mins        █░░░░░░░░░░░░░░░░░░░░░░░░   05.28 % 
Bash                     22 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.46 % 

🔥 Editors: 
Zsh                      12 hrs 43 mins      ████████████░░░░░░░░░░░░░   48.93 % 
VS Code                  10 hrs 24 mins      ██████████░░░░░░░░░░░░░░░   39.97 % 
Cursor                   1 hr 26 mins        █░░░░░░░░░░░░░░░░░░░░░░░░   05.53 % 
Obsidian                 1 hr 5 mins         █░░░░░░░░░░░░░░░░░░░░░░░░   04.21 % 
Vim                      21 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.37 % 

💻 Operating System: 
Linux                    26 hrs 1 min        █████████████████████████   100.00 % 
```


 Last Updated on 30/10/2024 00:52:39 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
