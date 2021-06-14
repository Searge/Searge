## Hi 👋, I'm Searge

### An artist passionate with code from Ukraine

<img src="https://komarev.com/ghpvc/?username=searge&label=Profile%20views&color=0e75b6&style=flat" alt="searge" />

- 🌱 I’m currently learning **Full Stack Web Development**

```python
"""Creating a class for keeping track of knowledge."""
import json
from pprint import pprint
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
    databases = ['SQLite', 'PostgreSQL', 'DynamoDB', 'Redis']
    misc = ['Linux', 'Shell', 'Docker', 'AWS']
    ongoing = ['Full Stack Web', 'Laravel', 'AWS']

    me = person('@Searge', 'Sergij Boremchuk',
                languages, databases, misc, ongoing)

    pprint(me.to_json())

# %%

```

### My Stats

[![Searge`s github stats](https://github-readme-stats.vercel.app/api?username=searge&show_icons=true&)](https://github.com/anuraghazra/github-readme-stats)

[![Searge's wakatime stats](https://github-readme-stats.vercel.app/api/wakatime?username=@Searge&layout=compact)](https://github.com/anuraghazra/github-readme-stats)

[![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=searge&layout=compact)](https://github.com/anuraghazra/github-readme-stats)
