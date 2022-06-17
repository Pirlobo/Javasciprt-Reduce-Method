# Javasciprt-Reduce-Method

// Online Javascript Editor for free
// Write, Edit and Run your Javascript code using JS Online Compiler


var human = [
    {id : 1, name : "A", gender : "nam"},
    {id : 2, name : "B", gender : "nam"},
    {id : 3, name : "C", gender : "nu"},
    {id : 4, name : "D", gender : "nu"},
    {id : 5, name : "E", gender : "nam"},
    ]
const output = human.filter((item) => item.gender === "nam")
.reduce((out, item) => {
    console.log(out)
    console.log(item)
    outp = {
        human : item.name + item.id,
        gender : item.gender
    }
    return [...out, outp]
}, [])

const numbers = [175, 50, 25];

console.log(numbers.reduce(myFunc))
console.log(numbers.reduce(myFunc, []))

function myFunc(total, num) {
//  	console.log(total)
// 	console.log(num)
  return total - num;
}


// Output

[]
{ id: 1, name: 'A', gender: 'nam' }
[ { human: 'A1', gender: 'nam' } ]
{ id: 2, name: 'B', gender: 'nam' }
[ { human: 'A1', gender: 'nam' },
  { human: 'B2', gender: 'nam' } ]
{ id: 5, name: 'E', gender: 'nam' }
100
-250
