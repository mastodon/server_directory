### Adding a Server File

The minimum valid Server File needs a `domain` and a `categories` field defined. The Filename has to match the `domain`
here is an example:

filename: `catland.meow.yaml`

```
---
domain: catland.meow
categories:
- food
- religion
```
A file with all possible fields set could look like this:

filename: `some.server.yaml`

```
---
domain: some.server
categories: [general]
legal_body_type: natural
region: europe
languages:
- en
- fr
description: on our server everyone is welcome, as long as you treat each other nicely and share pictures of your pets
```

### Schema definition
you can also find the schema definition here: .schema.yml

#### all fields explained:
- `categories` is a list and can be any number of the following values:
```
- academia
- activism
- adult
- art
- books
- food
- furry
- games
- general
- hobby
- humor
- journalism
- lgbt
- music
- bipoc
- regional
- religion
- sports
- tech
```

further you can define
- `legal_body_type` which can either be `natural` or `juridicial` 
- `region` which can either be `europe`, `north_america`, `south_america`, `africa`, `asia` or `oceania`

- `languages` and `description` are automatically pulled from the `languages` and `description` you have defined on your server, if you want to present your server with different `languages` or `description` you can define both here.
This will override the automatically pulled values on our end. 
`languages` is a list and can have multiple values from the following list:
```
- ar
- ast
- bg
- bn
- br
- ca
- co
- cs
- cy
- da
- de
- el
- en
- eo
- es
- et
- eu
- fa
- fi
- fr
- ga
- gl
- he
- hi
- hr
- hu
- hy
- id
- io
- is
- it
- ja
- ka
- kab
- kk
- kn
- ko
- lt
- lv
- mk
- ml
- mr
- ms
- nl
- nn
- no
- oc
- pl
- pt
- ro
- ru
- sk
- sl
- sq
- sr
- sv
- szl
- ta
- tai
- te
- th
- tr
- ug
- uk
- ur
- vi
- zh
```
