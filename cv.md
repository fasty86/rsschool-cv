# Oleg Tolmachev

## Bio:

- City: Moscow
- gender: Male
- age: 36

![](https://picsum.photos/200/300)

## Contacts:

- email: stepka86@gmail.com
- telegram: fasty86
- discord: Sailenthobo#9488

## About:

Graduated from MEPhi(Moscow Engineering Physics Institute) in 2009.

As a student start working as programmer in 1C consulting franchise. Soon after i switched to work with SAP ERP as BW/BI consultant,
also combine with a little of ABAP programming to resolve my task's.In late 2018 start working with SAP HANA and start learning SAP proprietary js framework SAPUI5 based on opensource framework OPENUi5.So i'm still working wit SAP.

I've always been interested in programming, so read some proggramming books in my free time , like "Elouqent JS" or "Python crash course" and finished cs50 course on edX platform.

## Skills and Proficiency:

- HTML5,CSS
- Javascript
- Git,Github
- ABAP
- IDE(WebStorm,VSCode,PyCharm)
- SQL
- Typescript basics
- Python basics

## Code example:

**Range Extraction:** _A format for expressing an ordered list of integers is to use a comma separated list of either individual integers
or a range of integers denoted by the starting integer separated from the end integer in the range by a dash, '-'. The range includes all integers in the interval including both endpoints. It is not considered a range unless it spans at least 3 numbers. For example "12,13,15-17"
Complete the solution so that it takes a list of integers in increasing order and returns a correctly formatted string in the range format._

```
function solution(list){
let result = []
	let formatted = []
	let current = []
	let last
	list.forEach(elem => {
		if (current.length == 0) {
			current.push(elem)
			last = elem
		} else {
			if (Math.abs(last - elem) == 1) {
				current.push(elem)
				last = elem
			} else {
				formatted.push(current)
				current = []
				current.push(elem)
				last = elem
			}
		}
	})
	formatted.push(current)
	formatted.map(elem =>{
		if (elem.length<3){
			elem.map(el => result.push([el]))
		}else{
			let range = []
			range.push(elem[0])
			range.push(elem.pop())
			result.push(range)
		}
	})
	//console.log(result.map(elem => elem.join('-')).join(','))
	return result.map(elem => elem.join('-')).join(',')
}
```

## Courses:

- cs50 on Edx.org

## Languages:

- English( reading fiction and non fiction books, listening podcast, watching youtube/movies, lack of speaking and writing practive )
- Russian( native )
