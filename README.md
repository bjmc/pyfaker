A python libary for generating pseudo-random (but "realistic") data.


Works with many languages and locales (the same as Ruby's Faker) so your fake data will be relevant to your location.

```
In [1]: from pyfaker import Fake

In [2]: fake = Fake(lang_code='en')

In [3]: fake.Address.street_address()
Out[3]: u'72449 Ward Shore'

In [4]: fake.Address.street_address()
Out[4]: u'7954 Waelchi Mall'

In [5]: fake.Company.bs()
Out[5]: u'whiteboard visionary markets'

In [6]: fake.Company.bs()
Out[6]: u'exploit innovative paradigms'

In [7]: fake.Name.name()
Out[7]: u'Aaliyah Bauch'

In [8]: fake.Name.name()
Out[8]: u"Chad O'Keefe"

In [9]: fake_de = Fake('de')

In [10]: fake_de.Address.street_address()
Out[10]: u'Imbacher Weg 471'

In [11]: fake_de.Address.city()
Out[11]: u'Schreiberdorf'

In [12]: fake_gb = Fake('en-gb')

In [13]: fake_gb.PhoneNumber.formats()
Out[13]: u'0800 906569'

In [14]: fake_gb.PhoneNumber.formats()
Out[14]: u'01662 12756'

```
*all of this is generated from the faker gem's yamls.*



####Next up:

- ~~python 3 support (!)~~
- make decorator (?) or apply to classes?
- guess what to fake based on names