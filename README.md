## Hi 👋, I'm Searge

### An artist passionate with code from Ukraine

<a href="https://stackoverflow.com/story/searge"><img src="https://img.shields.io/badge/stackoverflow-story-yellow?logo=stackoverflow" alt="StackOverflow Story" /></a> <img src="https://komarev.com/ghpvc/?username=searge&label=Profile%20views&color=0e75b6&style=flat" alt="searge" />

- 🌱 I’m currently learning **Full Stack Web Development**

```python
"""Creating a class for keeping track of knowledge."""
import json
from rich import print
from dataclasses import asdict, make_dataclass

person = make_dataclass('Person',
                        [('nick', str),
                         ('name', str),
                            ('languages', list[str]),
                            ('databases', list[str]),
                            ('misc', list[str]),
                            ('ongoing', list[str])],
                        namespace={
                            'to_json': lambda self: json.dumps(
                                asdict(self), indent=4)})
# %%

if __name__ == '__main__':
    languages = ['Python', 'JS', 'HTML', 'CSS', 'XPath', 'Lisp']
    databases = ['SQLite', 'PostgreSQL', 'Percona', 'DynamoDB', 'Redis']
    misc = ['Linux', 'Shell', 'LXC', 'Docker', 'AWS']
    ongoing = ['Full Stack Web', 'Magento 2 Cloud', 'AWS']

    me = person('@Searge', 'Sergij Boremchuk',
                languages, databases, misc, ongoing)

    print(me.to_json())

# %%

```
<sub>Thanks @rednafi for idea of script :wink:</sub>

### My Stats

[![Searge's github stats](https://github-readme-stats.vercel.app/api?username=searge&show_icons=true&theme=flag-india)](https://github.com/anuraghazra/github-readme-stats)

[![Searge's wakatime stats](https://github-readme-stats.vercel.app/api/wakatime?username=@Searge&layout=compact)](https://wakatime.com/@Searge)

[![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=searge&layout=compact)](https://github.com/anuraghazra/github-readme-stats)
