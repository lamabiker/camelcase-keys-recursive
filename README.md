
### Simple usage: 

	var camelGotHumps = camelCaseRecursive({'test-1':123, 'test-2':{'test-3:':{'test-four':132}}});

	//{ test1: 123, test2: { 'test3:': { testFour: 132 } } }
	console.log(camelGotHumps);

### Works with Arrays too:

	var anotherCamelWithTheHump = camelCaseRecursive({
		'test-1': 123,
		'test-Two': [{
			'test-three': {
				'test-FOUR': [{'test-five':[{testSix:{'test-seven':8}}]}]
			}
		}]
	});

	//{"test1":123,"testTwo":[{"testThree":{"testFour":[{"testFive":[{"testSix":{"testSeven":8}}]}]}}]}console.log(
	JSON.stringify(anotherCamelWithTheHump));

### More information on internal modules
Please refer to (camelcase)[https://www.npmjs.com/package/camelcase], (map-obj)[https://www.npmjs.com/package/map-obj] and (isarray)[https://www.npmjs.com/package/isarray] npm modules
