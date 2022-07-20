<p align="center">
    <img src="https://raw.githubusercontent.com/lnfel/wolf-summer-art/main/wolf-summer-hero.png" width="600" alt="WOLF SUMMER">
</p>

------

### About
This repository contains art for Wolf Summer: Haiku.

**Wolf Summer: Haiku** is a project for generating random Heroku-like names (generating random emails included).

Right now it only generates names and emails such as:
```
wolf-summer-1016
wolf.summer.1016@email-address.com
```

This is done by picking a random word from a pool of `adjectives` and `nouns` then appending a `hash` at the end of the combined words. This ensures that no generated haiku is similar to one another.

It can be fed by a custom pool of data to change the outcome of generated names or even generate a local version to your specific language.

The default hash uses numbers 0-9 and generates a 4 digit number that can be extended to your own desired liking. It can also opt in for a real hash-like output with letters, symbols and numbers combined.

The email's domain can also be customized to specific domain.

I am very satisfied with the outcome and will use this on our company's codebase as a utility.

### Roadmap
This is a pretty small project but I plan to expand the utilities to more than just a random names generator.

As you all have known [PHP Faker](https://github.com/fzaninotto/Faker) has been [sunsetted](https://github.com/fzaninotto/Faker/pull/2063#issuecomment-717118799) by it's author **François Zaninotto**. On his [blogpost](https://marmelab.com/blog/2020/10/21/sunsetting-faker.html) he mentioned:
> Faker Has A Design Problem
> 
> Because it embarks data for 70+ languages, including entire novels, Faker is a heavy library - more than 3MB.
> Developers like to use Faker for automated testing, so their CI server downloads it whenever someone opens a PR. As a consequence, Faker is used a lot.

With that in mind I intend to not make the same mistake as François did with Faker by not including localize files within the core project repo. Instead users can opt-in to use either the default or load a localized version of the data separately. This will ensure the package will only have a small foot-print.

I will update this repo soon for updates on this project.
Long Live Faker!