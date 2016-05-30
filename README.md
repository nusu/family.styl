**family.styl**
-------
## Version v1.0.4
this is port of [family.scss](https://github.com/LukyVj/family.scss) to stylus

**Installation:**

bower:

    $ bower install family.styl

git:

    $ git clone https://github.com/nusususuzu/family.styl.git

and import the mixin file:

    @import 'family.styl'

**Use the mixins:**

~~mixin name's are same as family.scss~~ , mixins are namespaced with "fm-" which comes from "family", **so if you want to use mixins in stylus you need to put "fm-" before every family mixin name**

Input:

    ul li
      background transparent
      +fm-first(3)
        background pink

Output:

    ul li {
      background: transparent;
    }
    ul li:nth-child(-n + 3) {
      background: pink;
    }

detailed mixin documentation:
  [family.scss](http://lukyvj.github.io/family.scss/)
