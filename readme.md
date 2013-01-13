# Grunt-Complexity

[Still a significant work in progress]

A [grunt](http://github.com/gruntjs/grunt/) task that utilizes
[complexity-report](https://github.com/philbooth/complexityReport.js)
to evaluate the complexity and maintainability of code.

## Usage

Within your grunt file:

```javascript
    // Project configuration.
	grunt.initConfig({

		complexity: {
			generic: {
				src: ['grunt.js', 'tasks/grunt-complexity.js'],
				options: {
					cyclomatic: 3,
					halstead: 8,
					maintainability: 100
				}
			}
		}
		

	});

	grunt.registerTask('default', 'complexity');
```

## What is Cyclomatic and Halstead?

Documentation on this to come.
