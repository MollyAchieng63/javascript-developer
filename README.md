# javascript-developer
# Question 2
var data = [[1,2,[3,4,[5,6],7,8,9]]]]
//[1,2,3,4,5,6,7,8,9]

var flatten = function(arr){
var flatMap = [];
arr.forEach(function(value){
	if(Array.isArray(value)){
	flatMap = flatMap.concat(flatten(value))
	}
	else{
	flatMap = flatMap.push(value)
	}
	});
	return flatMap;
	}
	var result = flatten(data);
	console.log(result);
	
	
	#Question 1
	
