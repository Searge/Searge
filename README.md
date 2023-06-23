# Hi, I'm Searge <img src="images/vulcan.webp" style="display: inline-block; margin: 0; height: 2rem" alt="Vulcan salute" />

## An DevOps Engineer at [Smile Ukraine](https://smile-ukraine.com/en)

![Visitors](https://komarev.com/ghpvc/?username=searge&label=Profile%20views&color=0e75b6&style=flat) [![Stand With Ukraine](https://raw.githubusercontent.com/vshymanskyy/StandWithUkraine/main/badges/StandWithUkraine.svg)](https://stand-with-ukraine.pp.ua)
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

[Skyline for 2021](https://skyline.github.com/Searge/2021)

<!--START_SECTION:waka-->
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C093%20hrs%2012%20mins-blue)

![Profile Views](http://img.shields.io/badge/Profile%20Views-1-blue)

**🐱 My GitHub Data** 

> 📦 216.6 kB Used in GitHub's Storage 
 > 
> 🏆 192 Contributions in the Year 2023
 > 
> 🚫 Not Opted to Hire
 > 
> 📜 59 Public Repositories 
 > 
> 🔑 9 Private Repositories 
 > 
**I'm an Early 🐤** 

```text
🌞 Morning                1210 commits        ██████░░░░░░░░░░░░░░░░░░░   22.19 % 
🌆 Daytime                2451 commits        ███████████░░░░░░░░░░░░░░   44.94 % 
🌃 Evening                1594 commits        ███████░░░░░░░░░░░░░░░░░░   29.23 % 
🌙 Night                  199 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.65 % 
```
📅 **I'm Most Productive on Saturday** 

```text
Monday                   782 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.34 % 
Tuesday                  729 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.37 % 
Wednesday                716 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.13 % 
Thursday                 781 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.32 % 
Friday                   785 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.39 % 
Saturday                 858 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.73 % 
Sunday                   803 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.72 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 7 hrs 33 mins       █████████████░░░░░░░░░░░░   51.03 % 
INI                      2 hrs 24 mins       ████░░░░░░░░░░░░░░░░░░░░░   16.29 % 
YAML                     1 hr 35 mins        ███░░░░░░░░░░░░░░░░░░░░░░   10.78 % 
Bash                     1 hr 22 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   09.29 % 
Other                    55 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   06.23 % 

🔥 Editors: 
VS Code                  8 hrs 10 mins       ██████████████░░░░░░░░░░░   55.20 % 
Obsidian                 6 hrs 6 mins        ██████████░░░░░░░░░░░░░░░   41.22 % 
Vim                      31 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.57 % 

🐱‍💻 Projects: 
Parma                    5 hrs 4 mins        █████████░░░░░░░░░░░░░░░░   34.21 % 
architecture             5 hrs               ████████░░░░░░░░░░░░░░░░░   33.81 % 
cdcintranet              2 hrs 13 mins       ████░░░░░░░░░░░░░░░░░░░░░   14.97 % 
notes                    1 hr 16 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   08.63 % 
Unknown Project          42 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.75 % 

💻 Operating System: 
Linux                    14 hrs 30 mins      ████████████████████████░   97.95 % 
Mac                      18 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.05 % 
```

**I Mostly Code in HTML** 

```text
Python                   9 repos             ████░░░░░░░░░░░░░░░░░░░░░   16.07 % 
PHP                      5 repos             ██░░░░░░░░░░░░░░░░░░░░░░░   08.93 % 
Shell                    4 repos             ██░░░░░░░░░░░░░░░░░░░░░░░   07.14 % 
Go                       3 repos             █░░░░░░░░░░░░░░░░░░░░░░░░   05.36 % 
Jinja                    3 repos             █░░░░░░░░░░░░░░░░░░░░░░░░   05.36 % 
```



**Timeline**

![Lines of Code chart](https://raw.githubusercontent.com/Searge/Searge/main/assets/bar_graph.png)


 Last Updated on 23/06/2023 21:56:41 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
