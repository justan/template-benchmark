# Node.JS template engines benchmark

[![Dependency Status](https://david-dm.org/justan/template-benchmark.png)](https://david-dm.org/justan/template-benchmark)

## Engines

- [CoffeeKup](https://github.com/mauricemach/coffeekup) v0.3.1 ([website](http://coffeekup.org/))
- [doT](https://github.com/olado/doT) v1.0.2 ([website](http://olado.github.com/doT/))
- [Dust](https://github.com/linkedin/dustjs) v2.2.2 ([website](http://linkedin.github.com/dustjs/))
- [Eco](https://github.com/sstephenson/eco) v1.1.0-rc-3
- [ECT](https://github.com/baryshev/ect) v0.5.5 ([website](http://ectjs.com/))
- [EJS](https://github.com/visionmedia/ejs) v0.8.5
- [Fest](https://github.com/mailru/fest) v0.8.0
- [Gaikan](https://github.com/Deathspike/gaikan) v1.3.13
- [Handlebars.js](https://github.com/wycats/handlebars.js/) v1.1.2 ([website](http://handlebarsjs.com/))
- [Hogan.js](https://github.com/twitter/hogan.js) v2.0.0 ([website](http://twitter.github.com/hogan.js/))
- [Jade](https://github.com/visionmedia/jade) v0.35.0 ([website](http://jade-lang.com/))
- [Swig](https://github.com/paularmstrong/swig) v1.2.2
- [Underscore](https://github.com/documentcloud/underscore) v1.5.2 ([website](http://underscorejs.org/))
- [Ant.js](https://github.com/antjs/ant.js) v0.2.1

## Test environment

- CPU: Intel Xeon E3-1230 V2 @ 3.3GHz
- OS: Windows 8.1
- Node.JS version: 0.10.21

## Results

	Rendering 100000 templates:

    Ant.js
      Escaped   : 12924ms
      Unescaped : 12856ms
      Total     : 25780ms

    Ant.js `.set`
      Escaped   : 2574ms
      Unescaped : 2583ms
      Total     : 5157ms

    ECT
      Escaped   : 3441ms
      Unescaped : 66ms
      Total     : 3507ms

    Dust
      Escaped   : 4751ms
      Unescaped : 629ms
      Total     : 5380ms

    Hogan.js
      Escaped   : 4544ms
      Unescaped : 422ms
      Total     : 4966ms

    Gaikan
      Escaped   : 3366ms
      Unescaped : 46ms
      Total     : 3412ms

    Fest
      Escaped   : 1480ms
      Unescaped : 151ms
      Total     : 1631ms

    EJS without `with`
      Escaped   : 5420ms
      Unescaped : 201ms
      Total     : 5621ms

    doT
      Escaped   : 2076ms
      Unescaped : 43ms
      Total     : 2119ms

    Swig
      Escaped   : 5603ms
      Unescaped : 223ms
      Total     : 5826ms

    Underscore
      Escaped   : 1836ms
      Unescaped : 1234ms
      Total     : 3070ms

    EJS
      Escaped   : 6545ms
      Unescaped : 976ms
      Total     : 7521ms

    Eco
      Escaped   : 6684ms
      Unescaped : 409ms
      Total     : 7093ms

    Handlebars.js
      Escaped   : 1767ms
      Unescaped : 219ms
      Total     : 1986ms

    Jade without `with`
      Escaped   : 6396ms
      Unescaped : 1987ms
      Total     : 8383ms

    CoffeeKup
      Escaped   : 2258ms
      Unescaped : 6567ms
      Total     : 8825ms

    Jade
      Escaped   : 7450ms
      Unescaped : 2948ms
      Total     : 10398ms


## Usage

	git clone git://github.com/baryshev/template-benchmark.git
	cd template-benchmark
	npm install
	node ./benchmark.js
